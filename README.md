Obrigatório 
Dupla negação e sarcasmo:
Nas mensagens que foram identificadas dupla negação e sarcasmo na classificação manual dos tweets, o nosso classificador não conseguiu interpretar qual o sentido que o usuário do twitter quer passar com a frase escrita, uma vez que ele imputa apenas a probabilidade de tal palavra pertencer a lista de palavras relevantes ou irrelevantes.
Futuramente, pode ser desenvolvido um sistema de inteligência artificial, esse sistema poderá encontrar padrões nas sequências de palavras não levando em conta somente a probabilidade de cada palavra individual, por exemplo, na frase “Mas que rápida essa entrega da nubank…”  será calculada a probabilidade da frase ocorrer exatamente nessa sequência de palavras. Uma forma de expandir seria implementar inteligência artificial ao classificador, entrando na conta do usuário que escreveu o tweet e verificar se ele costuma escrever tweets relevantes ou não, e então acrescentar essa probabilidade para aumentar a probabilidade do tweet sobre nubank ser relevante ou não.


Opcional 
O classificador precisa de uma base para comparar a quantidade de acerto ou a sua eficiência em relação aos tweets relevantes e irrelevantes, ou seja, é preciso classificar antes o que é relevante ou não, para que depois de feito o classificado verificar o quão eficiente ele foi. Ou seja isso é para evitar o overfitting [explicar o que é overfitting], pois senão o classificador será satisfatório com as palavras que ele já viu, no entanto, se for testado com palavras que ele nao viu, ele terá um resultado não satisfatório(uma boa quantidade de acerto do classificador em relação a relevância do tweet). 

Um cenário diferente que o nosso classificador poderia ser implementado seria para  filtrar currículos para entrevista de uma empresa. Por exemplo uma empresa quer ver quais candidatos se encaixam para determinado cargo, o classificador irá separar tais candidatos pelas características que a empresa procura, e assim, aqueles que irão para a entrevista serão os mais propício a ocupar o cargo segundo as características buscadas. Outro cenário que também poderia ter o classificador, seria usar ele para classificar os e-mails como spam ou não, os guardando na caixa de spam. Assim corrigindo o erro de muitos e-mails que são importantes irem para caixa de spam sem o usuário saber.

A melhoria que poderia ser implementada no classificador seria considerar palavras juntas e não apenas separadas, por exemplo “O cartão de natal”, nesse caso não estaríamos falando de cartão de crédito e sim de um cartão de uma comemoração, logo, nosso classificador olharia quais palavras iriam aparecer após cartão, verificando assim a probabilidade de se tratar de um cartão de crédito e não outro qualquer. No antigo, ele iria apenas ver que a probabilidade da palavra cartão seria alta, então, a probabilidade da frase seria alta também, o que seria errado pois não é sobre cartão de crédito, assim, no código antigo essa frase provavelmente seria relevante. Todas essas melhorias poderiam ser aplicadas com Machine Learning, onde o classificador poderia aprender uma sequência de palavras e considerar isso para classificar os tweets como relevantes, evitando erros como esse exemplo do cartão que não é de crédito.
