
#  DER + Banco de Dados do blog pessoal 

## 1 - Visualização do DER
[Para visualizar o DER clique aqui](https://dbdesigner.page.link/11aRwfjVX6hDdwAN7)

[Para visualizar a versão PDF clique aqui](https://github.com/anagjorge/Exercicios_SQL/blob/main/Blog-dbdesigner.pdf)

![DER](https://github.com/anagjorge/DER_blogPessoal/blob/main/DER_Image.png)

## 2 - Dicionário de dados 

<div>

### Postagens 
 
<table>
  <thead>
    <th> Restrições de domínio </th>
    <th> Atributos</th>
    <th> Tipo de dado</th>
    <th> Tamanho </th>
    <th> Descrição </th>
  </thead>
  <tbody>
    <tr>
      <td>PK | Not Null </td>
      <td> Id </td>
      <td> bigint</td>
      <td></td>
      <td>Código de identificação da tabela Postagens</td>
    <tr>
      <td> Not null </td>
      <td> Titulo </td>
      <td> Varchar </td>
      <td>255</td>
      <td>Titulo das Postagens</td>
    </tr>
    <tr>
      <td>Not Null</td>
      <td> Texto </td>
      <td> Varchar </td>
      <td> 1000 </td>
      <td>Textos das Postagens</td>
    </tr>
    <tr>
      <td>Not Null</td>
      <td> Data </td>
      <td> Timestamp </td>
      <td></td>
      <td>Representação da data e do horário atual levando em consideração o fuso horário</td>
    </tr>
    <tr>
      <td>FK | Not Null</td>
      <td> tema_id  </td>
      <td> bigint </td>
      <td></td>
      <td>Chave estrangeira referenciando o código da tabela Temas </td>
    </tr>
    <tr>
      <td>FK | Not Null</td>
      <td> usuario_id </td>
      <td> bigint </td>
      <td></td>
      <td>Chave estrangeira referenciando o código da tabela Temas</td>
    </tr>
  </tbody>
</table>

### Temas
<table>
  <thead>
    <th> Restrições de domínio </th>
    <th> Atributos</th>
    <th> Tipo de dado</th>
    <th> Tamanho </th>
    <th> Descrição </th>
  </thead>
  <tbody>
    <tr>
      <td>PK </td>
      <td> Id </td>
      <td> bigint</td>
      <td></td>
      <td>Código de identificação da tabela Temas</td>
    <tr>
      <td>Not Null</td>
      <td> Descricao </td>
      <td> Varchar </td>
      <td>255</td>
      <td> Descrição do tema </td>
    </tr>
  </tbody>
</table>

### Usuário
<table>
  <thead>
    <th> Restrições de domínio </th>
    <th> Atributos</th>
    <th> Tipo de dado</th>
    <th> Tamanho </th>
    <th> Descrição </th>
  </thead>
  <tbody>
    <tr>
      <td>PK</td>
      <td> Id </td>
      <td> bigint</td>
      <td></td>
      <td>Código de identificação da tabela Usuário</td>
    <tr>
      <td>Not Null</td>
      <td> Nome </td>
      <td> Varchar </td>
      <td>255</td>
      <td> Nome dos usuários</td>
    </tr>
    <tr>
      <td>Not Null</td>
      <td> Usuario </td>
      <td> Varchar </td>
      <td>255</td>
      <td> Login do usuário </td>
    </tr>
    <tr>
      <td>Not Null</td>
      <td> Senha </td>
      <td> varchar </td>
      <td>255</td>
      <td>Senha do usuário</td>
    </tr>
  </tbody>
</table>
</div>
<br>

## 3 - Código SQL 
![SQL](https://github.com/anagjorge/blogPessoal-backend/blob/master/Documenta%C3%A7%C3%A3o/Codigo_SQL_Image.png)
