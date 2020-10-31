# devops_ac05  
***Atividade Contínua 05***  

***Estilo de código SQL***
--------------------------------------------------  

***Arquivo requirements.txt***  

![print01](https://github.com/MS-Oliveira/devops_ac05/blob/main/imagens_AC5/print01.PNG)  

_Demonstra qual os requisitos do ambiente para projetos._  

------------------------------------------------------------  

***Editor SQL com script de teste (antes de aplicar o estilo de código)***  

1. Criar ambiente virtual (venv): python -m venv /caminho da pasta/venv  
2. Ativar o venv: source venv/Scripts/activate  
3. pip3 install sqlfluff  
4. pip freeze > requirement.txt : para criar os requisitos do ambiente    
5. echo "  SELECT a  +  b FROM tbl;  " > teste.sql (criando arquivo SQL para teste)  
6. cat teste.sql : apresenta no bash os dados contidos no arquivo (_print abaixo_) 


![print02](https://github.com/MS-Oliveira/devops_ac05/blob/main/imagens_AC5/print02.PNG)  


------------------------------------------------------------   

***Apresentando as não conformidades***   

7. sqlfluff lint teste.sql : testa o estilo do código  (caso o teste apresente erro mostrará a linha com erro, como no print abaixo)  
 

![print03](https://github.com/MS-Oliveira/devops_ac05/blob/main/imagens_AC5/print03.PNG)  

***Demonstra qual linha apresenta erro.***  

------------------------------------------------------------  

***No editor para correção do código SQL***       

8. vim teste.sql (abre o editor no bash)  
9. Caso não esteja na opção INSERT, aperte a tecla "i" e permitirá a correção dos dados.  
10. Após a edição aperte a tecla "Esc" e em seguida ':wq' para salvar e fechar o editor.  

![print04](https://github.com/MS-Oliveira/devops_ac05/blob/main/imagens_AC5/print04.PNG)  

***Código após edição.***  

-------------------------------------------------------------------  

***No Shell mostrando o teste após as correções***       

11. sqlfluff lint teste.sql : testa o estilo do código  (caso passe no teste apresenta uma tela semelhante ao print abaixo)  
   

![print05](https://github.com/MS-Oliveira/devops_ac05/blob/main/imagens_AC5/print05.PNG)  

***Código passou no teste de estilo de código ideal para SQL.***  

-----------------------------------------------------------------------

***Fontes***  
 
Dicas para o editor Vim: https://medium.com/tableless/comandos-b%C3%A1sicos-do-vim-para-ningu%C3%A9m-ficar-preso-no-servidor-93f0d21d5508  

Passo a passo da ferramenta SQLFluff: https://docs.sqlfluff.com/en/latest/  




