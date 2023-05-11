sns.set_style("whitegrid")
sns.set_palette("Set2")

plt.figure(figsize=(10, 6))
sns.scatterplot(data=df_results, x='predicted', y='actual', hue='deciles', alpha=0.8, s=100)
sns.lineplot(data=df_grouped, x='predicted', y='actual', color='red', linewidth=2, marker='o')

plt.title("Actual vs Predicted Values by Deciles")
plt.xlabel("Predicted Values")
plt.ylabel("Actual Values")
plt.legend(title="Deciles", loc='upper left', bbox_to_anchor=(1.05, 1))

plt.show()

data have;

   input date1 date9. date2 date9.;

   format date1 date2 date9.;

   datalines;

01JAN2022 15JAN2022

15FEB2022 25FEB2022

;

data want;

   set have;

   do i = 0 to intck('day',date1,date2);

      date3 = intnx('day',date1,i);

      output;

   end;

   format date3 date9.;

   drop i;

run;
