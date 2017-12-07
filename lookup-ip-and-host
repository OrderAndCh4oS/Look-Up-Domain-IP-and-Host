import socket
# from domain_list import domains

domains = [
    'google.com',
    'facebook.com'
]

def lookupIp(domain, f):
    print(domain)
    try :
        host = socket.gethostbyaddr(domain)
        f.write(domain + ', ' + host[2][0] + ', ' + host[0] + '\r')
    except:
        f.write(domain + ', oh no an exception, oh no an exception' + '\r')

f = open('ips.csv', 'w')
for d in domains:
    lookupIp(d, f)
f.close()
print('Fin')
