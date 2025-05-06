# codes-
for me and betul 
df['cfe'] = df['cfe'].fillna(df['dif'].apply(lambda x: 'O' if pd.notna(x) else 'N'))
# Step 1: Keep original dif, no imputation
# Step 2: Add a closure status column
df['is_closed'] = df['dif'].notna()

# Optional: Impute dif for technical reasons
df['dif_imputed'] = df['dif'].fillna(pd.to_datetime('2099-12-31'))
