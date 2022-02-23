# Comandos dotnet entity framework
<br/>


## Gerar views em dotnet

   
    //Com SQLLite
    dotnet-aspnet-codegenerator controller -name ProdutoController -dc AppDbContext -m Models.Traducao.Produtos --useDefaultLayout --useSqlite --referenceScriptLibraries
    
    //Sem SQLLite
    dotnet-aspnet-codegenerator controller -name ProdutoController -dc AppDbContext -m Models.Traducao.Produtos --useDefaultLayout --referenceScriptLibraries
    

07391798452@aranet.net.br

# Migrations

    # contexto padrão
    dotnet ef migrations add Inicial --context AppDbContext

    # contexto diferente
    dotnet ef migrations add Inicial --context AuthDbContext
