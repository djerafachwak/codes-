# codes-
for me and betul 



df['dif'] = df['dif'].fillna(pd.to_datetime('2099-12-31'))

df['is_closed'] = df['dif'] != pd.to_datetime('2099-12-31')

df['dif'] = df['dif'].fillna(pd.to_datetime('2099-12-31'))

df['residence'] = df['residence'].fillna('Non Reside')

df.loc[df['dco'].isna() & df['Lib_ope'].isna(), 'Lib_ope'] = 'No reactivation'


df['dco'] = df['dco'].fillna(pd.to_datetime('2099-12-31'))

df['is_reactivated'] = df['dco'] != pd.to_datetime('2099-12-31')



