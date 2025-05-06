# codes-
for me and betul 
df['cfe'] = df['cfe'].fillna(df['dif'].apply(lambda x: 'O' if pd.notna(x) else 'N'))

df['is_closed'] = df['dif'].notna()

df['dif'] = df['dif'].fillna(pd.to_datetime('2099-12-31'))
df['is_closed'] = df['dif'] != pd.to_datetime('2099-12-31')
