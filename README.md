# codes-
for me and betul 
df['cfe'] = df['cfe'].fillna(df['dif'].apply(lambda x: 'O' if pd.notna(x) else 'N'))
