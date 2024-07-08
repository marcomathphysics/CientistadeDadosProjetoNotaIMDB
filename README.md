# CientistadeDadosProjetoNotaIMDB

Para executar o projeto precisa fazer download do arquivo modeloIMDB.pkl e usar o seguinte codigo:



    import pickle
    with open("modeloIMDB.pkl", "rb") as arquivo:
		   modelo = pickle.load(arquivo)
    import pandas as pd
    previsao = modelo.predict(DATA)
    print(previsao)

    
	

 A DATA for input  can be an N-row dataframe, where the list of  column is as follow:
 ['Released_Year', 'Runtime', 'Meta_score', 'No_of_Votes', 'Gross',
       'Biography', 'Family', 'Film-Noir', 'Horror', 'Romance', 'Sci-Fi',
       'Drama', 'Fantasy', 'Comedy', 'Mystery', 'War', 'Animation', 'Crime',
       'Thriller', 'Action', 'Musical', 'Music', 'Adventure', 'History',
       'Sport']


       
 For example for the movie The Shawshank Redemption  we can have the DATA for input as follows:      
 x0data={'Released_Year': [1994],
 'Runtime': [142],
 'Meta_score': [80.0],
 'No_of_Votes': [2343110],
 'Gross': [28341469],
 'Biography': [0],
 'Family': [0],
 'Film-Noir': [0],
 'Horror': [0],
 'Romance': [0],
 'Sci-Fi': [0],
 'Drama': [1],
 'Fantasy': [0],
 'Comedy': [0],
 'Mystery': [0],
 'War': [0],
 'Animation': [0],
 'Crime': [0],
 'Thriller': [0],
 'Action': [0],
 'Musical': [0],
 'Music': [0],
 'Adventure': [0],
 'History': [0],
 'Sport': [0]}   


import pandas as pd

DATA = pd.DataFrame(x0data)

