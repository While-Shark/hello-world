#coding=utf-8
import string
from hashlib import md5

a = string.ascii_letters + string.digits
# a = abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789

for a1 in a:
    for a2 in a:
        for a3 in a:
            for a4 in a:
                str = a1 + a2 + a3 + a4 + 'LiHua'
                if '1a4fb3fb5ee' in md5(str).hexdigest():
                    print(a1 + a2 + a3 + a4 + 'LiHua')
                    break

