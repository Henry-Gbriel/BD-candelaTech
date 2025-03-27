<h1>📌 CandelaTech - Gerenciamento de Projetos</h1>
    
<h2>📖 Descrição</h2>

<p>O <strong>CandelaTech</strong> é um banco de dados projetado para gerenciar informações sobre clientes, desenvolvedores, projetos e materiais utilizados. Esse sistema facilita o controle de orçamentos, status de projetos e aprovações.</p>
    
<h2>🛠️ Estrutura do Banco de Dados</h2>
<ul>
    <li><strong>Cliente</strong>: Armazena informações pessoais e de contato dos clientes.</li>
    <li><strong>Desenvolvedor</strong>: Registra os dados dos desenvolvedores responsáveis pelos projetos.</li>
    <li><strong>Projeto</strong>: Contém informações sobre os projetos, incluindo dimensões, orçamento e status.</li>
    <li><strong>Material</strong>: Lista os materiais utilizados nos projetos, seus fornecedores e preços.</li>
    <li><strong>Projeto_Material</strong>: Relaciona os materiais utilizados em cada projeto.</li>
    <li><strong>Aprovação</strong>: Armazena registros de aprovação de projetos pelos clientes.</li>
</ul>
    
<h2>📄 Função de Cada Item</h2>
<ul>
    <li><strong>Cliente</strong>: Registra os dados básicos dos clientes que solicitam projetos.</li>
    <li><strong>Desenvolvedor</strong>: Mantém os dados dos profissionais responsáveis pelo desenvolvimento dos projetos.</li>
    <li><strong>Projeto</strong>: Armazena detalhes como altura, largura, peso máximo, orçamento e status do projeto.</li>
    <li><strong>Material</strong>: Define os materiais usados nos projetos, com nome, fornecedor e preço.</li>
    <li><strong>Projeto_Material</strong>: Relaciona quais materiais foram usados em determinado projeto, incluindo quantidade.</li>
    <li><strong>Aprovação</strong>: Registra a data de aprovação do projeto e os envolvidos (cliente e projeto).</li>
</ul>


<h2>🏗️ Modelo Lógico e Conceitual</h2>
<p>O modelo lógico e conceitual do banco de dados representam a estrutura e os relacionamentos entre as tabelas. Adicione as imagens ou diagramas para facilitar a compreensão:</p>
<img src="https://github.com/user-attachments/assets/f230e29a-2095-4ea8-93e0-6b1bda0d0cb0" alt="Modelo Conceitual">
<br>
<br>
<img src="https://github.com/user-attachments/assets/40b98e36-d165-4f50-b851-adbd615910d7" alt="Modelo Lógico">

    
<h2>📄 Explicação dos Caracteres e Atributos das Tabelas</h2>
<ul>
    <li><strong>VARCHAR(N)</strong>: Usado para armazenar texto de tamanho variável. O "N" define o número máximo de caracteres. Exemplo: `VARCHAR(255)` armazena até 255 caracteres.</li>
    <li><strong>TEXT</strong>: Usado para armazenar textos maiores, sem limite de tamanho pré-definido.</li>
    <li><strong>BIGINT</strong>: Um tipo de dado numérico usado para armazenar números inteiros grandes. Ideal para IDs ou quantidades muito altas.</li>
    <li><strong>DECIMAL(X, Y)</strong>: Usado para armazenar valores numéricos com ponto flutuante (como valores monetários). O "X" define o total de dígitos e "Y" define a quantidade de casas decimais. Exemplo: `DECIMAL(10,2)`.</li>
    <li><strong>ENUM('valor1', 'valor2', 'valor3')</strong>: Usado para definir um conjunto fixo de valores possíveis para uma coluna. Exemplo: `ENUM('pendente', 'aprovado', 'cancelado')`.</li>
    <li><strong>TIMESTAMP</strong>: Armazena data e hora do evento (geralmente de criação ou atualização). Por exemplo: `TIMESTAMP DEFAULT CURRENT_TIMESTAMP` armazena automaticamente a data e hora de criação do registro.</li>
    <li><strong>PRIMARY KEY</strong>: Define a coluna como chave primária, ou seja, um identificador único para cada registro na tabela. Não pode haver valores duplicados nesta coluna.</li>
    <li><strong>FOREIGN KEY</strong>: Define uma chave estrangeira, criando um vínculo entre duas tabelas. Garante integridade referencial e que os dados em uma tabela estão associados a registros válidos de outra tabela.</li>
    <li><strong>NOT NULL</strong>: Indica que a coluna não pode ter valor nulo. Ou seja, o valor deve ser fornecido ao inserir ou atualizar registros.</li>
    <li><strong>UNIQUE</strong>: Garante que os valores em uma coluna sejam únicos dentro da tabela. Não pode haver valores duplicados nesta coluna.</li>
    <li><strong>DEFAULT</strong>: Define um valor padrão para a coluna caso nenhum valor seja fornecido no momento da inserção de dados. Exemplo: `DEFAULT CURRENT_TIMESTAMP` para registrar a data e hora de criação automaticamente.</li>
</ul>
    
    
<h2>🚀 Tecnologias Utilizadas</h2>
<ul>
    <li><strong>MySQL</strong> - Banco de dados relacional</li>
    <li><strong>SQL</strong> - Linguagem para manipulação do banco de dados</li>
</ul>
    
<h2>📄 Licença</h2>
<p>Este projeto está licenciado sob a <a href="LICENSE">MIT License</a>.</p>
    
<h2>🤝 Contribuição</h2>
<p>Fique à vontade para abrir issues e enviar pull requests para melhorias no projeto!</p>
    
<h2>📞 Contato</h2>
<p>Caso tenha dúvidas ou sugestões, entre em contato:</p>
<ul>
    <li>📧 Email: <a href="mailto:santossilvahenrygabriel58@gmail.com">Meu email de contato</a></li>
    <li>🔗 LinkedIn: <a href="www.linkedin.com/in/henry-gabriel-santos-silva-6ba776209">Meu Perfil linkedin</a></li>
</ul>
    
<hr>
    
<p>⭐ Se gostou do projeto, deixe um star no repositório!</p>

</body>
</html>

 
