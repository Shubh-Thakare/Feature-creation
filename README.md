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
