### Chall Desc:
My friend made this encryption scheme using matrices but he didn't make the decryption scheme, Please help me decrypt this message!

### File attached: chall.py
```py
flag = 'REDACTED'
rand = 'Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹Ô¹'
def str_to_matrix(string):
    for i in range(2):
        letter = ord(string)
        flag_mat = [letter,letter]
        return flag_mat
final_flag_matrix = []
for i in flag:
    final_flag_matrix.append(str_to_matrix(i))
leet_matrix = []
for i in rand:
    leet_matrix.append(str_to_matrix(i))
enc_flag_matrix = []
for i in final_flag_matrix:
        x = int(i[0]) * int(i[1])
        enc_flag_matrix.append(x)
enc_leet_matrix = []
for i in leet_matrix:
    y = int(i[0]) * int(i[1])
    enc_leet_matrix.append(y)
print(f'leet={enc_leet_matrix}')
print('='*80)
final_ct = []
for i in range(len(enc_leet_matrix)):
        final_ct.append(enc_leet_matrix[i]*enc_flag_matrix[i])
print(f'ct={final_ct}')
#ct=[21629584900, 4118558976, 4118558976, 17167812676, 26606176996, 27044131401, 5407396225, 19334346304, 4291953169, 23640600025, 16132810225, 23640600025, 17519963769, 19334346304, 4649466969, 21238107289, 4649466969, 16132810225, 24053528464, 4118558976, 4118558976, 20465877481, 16132810225, 21238107289, 4649466969, 16132810225, 21238107289, 4118558976, 23231246724, 4649466969, 16132810225, 24053528464, 19334346304, 4833586576, 21629584900, 16132810225, 18597867876, 4291953169, 24890110756, 4649466969, 16132810225, 19334346304, 4118558976, 24470032041, 23231246724, 23640600025, 16132810225, 24053528464, 4118558976, 16132810225, 21238107289, 4833586576, 20465877481, 4649466969, 16132810225, 4833586576, 21629584900, 17875690000, 16132810225, 5021281321, 16132810225, 21238107289, 4291953169, 21629584900, 24470032041, 24053528464, 4649466969, 23640600025, 16132810225, 24053528464, 4118558976, 16132810225, 23640600025, 4118558976, 20850204816, 24890110756, 4649466969, 16132810225, 25740993600, 8265719056, 8265719056, 27930765625]
```

In progress.....
