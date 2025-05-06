# codes-
for me and betul 



df['dif'] = df['dif'].fillna(pd.to_datetime('2099-12-31'))

df['is_closed'] = df['dif'] != pd.to_datetime('2099-12-31')

df['dif'] = df['dif'].fillna(pd.to_datetime('2099-12-31'))

df['residence'] = df['residence'].fillna('Non Reside')

