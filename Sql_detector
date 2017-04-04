import requests

def titulo():
    print('''
    
  _____       _   _____        _            _             
 / ____|     | | |   __ \     | |          | |            
| (___   __ _| | |  |  | | ___| |_ ___  ___| |_ ___  _ __ 
 \___ \ / _` | | |  |  | |/ _ \ __/ _ \/ __| __/ _ \| '__|
 ____) | (_| | | |  |__| |  __/ ||  __/ (__| || (_) | |   
|_____/ \__, |_| |______/ \___|\__\___|\___|\__\___/|_|   
           | |                                         
           |_|         
#==========================================================#

					By: Felipe Tesão
					
#==========================================================#    
    ''')

teste="%27"

while True:
    titulo()
    print("Exemplo: www.site.com/loja.php?id=20\n")
    site = input("Digite o site: ")
    url = "http://" + site + teste

    print("A url será essa:"+url)


    req=requests.get(url)

 
    if(req.status_code != 200):
    	print("Erro de conexão")

    if("mysql_fetch_array()" in req.text or "You have an error in your SQL" in req.text):
    	print("\n\n        SITE VULNERAVEL\n\n")

    else:
    	print("\n\n        Site nao vulneravel! :(\n\n")


