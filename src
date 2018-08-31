#######################
#                     #
#   ***DARK_LIST***   #
#  Augusto Fadanelli  #
#  Date: 29/08/2018   #
# Version: 0.0.1 beta #
#                     #
#######################

# Bibliotecas
import os.path

print('\t***DARK_LIST***\n\tV0.0.1 beta')

# Variáveis
var_about = 'Created by: Augusto Fadanelli de Sousa\nEmail: augustofadanelli2016@gmail.com'
var_help = 'about\tMostra detalhes\nlist\tCria listas de dicionário'
cont = False
local = 'C:\Program Files\darklist\path.txt'

# Cria arquivo que define pasta padrão onde será salvo as listas
bool_local = os.path.exists(local)
if bool_local == False:
    path = input('(local_save_lists)>> ')
    os.makedirs(local) # Cria diretório local
    # Adiciona path ao arquivo path.txt
    file = open(local, 'w')
    file.write(path)
    file.close()

    bool_path = os.path.exists(path)
    if bool_path == False:
        os.makedirs(path) # Cria diretório path

while cont == False:

    command = input('>> ')

    if command == 'about':
        print(var_about)
    elif command == 'help':
        print(var_help)

    elif command == 'list':
        var_list = input('(list)>> ')
        if var_list != '--exit' and var_list != '--quit':
            var_list_split = var_list.split('.')
            # name = input('(list>name)>>')
            # file = open(path + name, 'w')
            # file.write(var_list_split)
            # file.close()
            print(var_list_split)  # apagar
            # print(var_list_split[0] + var_list_split [1] + var_list_split [2]) #apagar
        elif var_list == '--quit':
            cont = True

    # Deixar sempre por ultimo
    elif command != 'quit':
        print('ERROR: Command not found.')

    if command == 'quit':
        cont = True
    command = ''
