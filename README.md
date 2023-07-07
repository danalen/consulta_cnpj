# consulta_cnpj
Consultar CNPJ na base da SEFAZ

<div class="card-header">Campos de retorno da API <strong>SINTEGRA</strong></div>

| Campo       | Tipo       | Descrição                                         |
|-------------|------------|---------------------------------------------------|
| abertura    | String     | Data da situação cadastral no formato dd-MM-yyyy. |
| situacao    | String     | Situação Cadastral da Inscrição Estadual (IE) no Sintegra: Valores possíveis: `**Ativo**` `**Inativo**` `**Baixado**`|
| tipo        | String     | Filial/Matriz |
| nome        | String     | Razão social. |
| fantasia    | String     | Nome Fantasia |
| porte       | String     | Porte da empresa |
