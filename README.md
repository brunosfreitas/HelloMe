HelloMe
=======

Para o inicio do projeto segui as guidelines em 
  http://developer.android.com/training/basics/firstapp/index.html
  
Logo após foi criada uma guideline com as metricas e cores no photoshop
https://github.com/brunosfreitas/HelloMe/blob/master/guideline%20copy.png
 
Para seguir com um código organizado todas as questoes de posicionamento, tamanho e textos foram postos em código
  
Segui a ideia de colocar o tamanho de itens em porcentagens, para isto foi necessario modificar o layout para LinearLayout
 http://stackoverflow.com/questions/4961355/percentage-width-in-a-relativelayout
  
Houve um problema entre o LinearLayout (o qual aceita porcentagens mas não alinhamento vertical) vs RelativeLayout (que aceita alinhamento vertical mas não porcentagens). Seguimos com o RelativeLayout e valor fixo de largura. Existia a opção de aninhar um Linear comn um Relative mas a solução pareceu pesada demais para o proposto
  
Após isto avançamos para a action do clique button_clicked, seguindo
 http://developer.android.com/training/basics/firstapp/starting-activity.html
foi extremamente facil criar a proxima tela, só ajustando o tamanho da label, com o avanço disto descobri que poderia colocar as metricas no arquivo dimens.xml.
 
Mesmo tendo "concluido" o pedido, ainda senti que fixando um valor de largura aos itens poderia ocasionar em diferentes tipos de comportamentos em dispositivos diferentes (se a tela for muito grande o botao vai ficar pequeno dentro da tela) entao resolvi trabalhar com paddings em vez de largura. 

