Este script em Python facilita a extração de dados de um banco de dados SQL Server e os salva em arquivos CSV. 

Ele utiliza a biblioteca pyodbc para conectividade com o banco de dados e pandas para manipulação de dados. O processo envolve conectar-se ao SQL Server, atualizar a tabela, se necessário, executar uma consulta SQL para recuperar os dados e, em seguida, dividir e salvar os resultados em arquivos CSV.

Recursos Principais:

### Funções Modulares:

Conectar ao SQL Server: Estabelece uma conexão com o banco de dados SQL Server usando a biblioteca pyodbc.
Atualizar Tabela: Executa uma stored procedure para atualizar a tabela, se necessário.
Dividir Resultados: Divide os dados recuperados em lotes gerenciáveis para evitar sobrecarga de memória.
Salvar em CSV: Salva os lotes de dados em arquivos CSV separados.

### Personalização:

Os usuários podem modificar a consulta SQL e especificar o número máximo de linhas por arquivo CSV.
Os caminhos do diretório de saída podem ser personalizados conforme as necessidades do usuário.

### Tratamento de Erros:

Fornece tratamento de erros para problemas de conexão e erros na execução do SQL.

### Uso:

Configure os parâmetros de conexão com o SQL Server (Server, Database, etc.).
Especifique a consulta SQL para recuperar os dados desejados.
Defina o número máximo de linhas por arquivo CSV (max_rows_per_file).
Defina o diretório de saída base para os arquivos CSV (base_output_directory).
Execute o script para conectar-se ao SQL Server, atualizar a tabela (se necessário), recuperar dados e salvá-los em arquivos CSV.

### Dependências:

pyodbc: Para conectividade com o SQL Server.
pandas: Para manipulação de dados (não é usada diretamente neste script, mas pode ser útil para processamento adicional de dados).


### Observação:

Certifique-se de que os drivers apropriados estejam instalados e configurados para pyodbc se conectar ao SQL Server.
