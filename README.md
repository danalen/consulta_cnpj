# consulta_cnpj
Consultar CNPJ na base da SEFAZ

<div class="card-header">Campos de retorno da API <strong>SINTEGRA</strong></div>
<table class="table table-sm table-hover table-bordered table-striped">
           <thead>
              <tr>
                 <th>Campo</th>
                 <th>Tipo</th>
                 <th>Descrição</th>
              </tr>
           </thead>
           <tbody>
              <tr>
                <td><strong>status</strong></td>
                <td>string</td>
                <td>Indica a situação da requisição.<br>
                  <strong style="color: #404040;">Valores possíveis</strong>:
                  <ul style="padding-left: 18px; padding-top: 10px;">
                    <li><code>OK</code></li>
                    <li><code>ERROR</code></li>
                  </ul>
                </td>
              </tr>
              <tr>
                <td><strong>code</strong></td>
                <td>string</td>
                <td>Código de retorno utilizado para informar o status da requisição.</td>
              </tr>
              <tr>
                 <td><strong>message</strong></td>
                 <td>string</td>
                 <td>Mensagem explicativa indicando o campo <em>status</em>.</td>
              </tr>
              <tr>
                 <td><strong>cnpj</strong></td>
                 <td>string</td>
                 <td>CNPJ no formato <em>00000000000000</em>.</td>
              </tr>
              <tr>
                 <td><strong>nome_empresarial</strong></td>
                 <td>string</td>
                 <td>Razão social.</td>
              </tr>
              <tr>
                 <td><strong>nome_fantasia</strong></td>
                 <td>string</td>
                 <td>Nome fantasia.</td>
              </tr>
              <tr>
                 <td><strong>inscricao_estadual</strong></td>
                 <td>string</td>
                 <td>Inscrição Estadual.</td>
              </tr>
              <tr>
                 <td><strong>tipo_inscricao</strong></td>
                 <td>string</td>
                 <td>Tipo de Inscrição Estadual.</td>
              </tr>
              <tr>
                 <td><strong>data_situacao_cadastral</strong></td>
                 <td>string</td>
                 <td>Data da situação cadastral no formato dd-MM-yyyy.</td>
              </tr>
              <tr>
                 <td><strong>situacao_cnpj</strong></td>
                 <td>string</td>
                 <td>Situação cadastral do CNPJ.</td>
              </tr>
              <tr>
                 <td><strong>situacao_ie</strong></td>
                 <td>string</td>
                 <td>Situação Cadastral da <strong>Inscrição Estadual</strong> (IE) no <strong>Sintegra</strong>: <br> 
                  <strong style="color: #404040;">Valores possíveis</strong>:
                  <ul style="padding-left: 18px; padding-top: 10px;">
                    <li><code>Ativo</code></li>
                    <li><code>Inativo</code></li>
                    <li><code>Baixado</code></li>
                  </ul>
                 <!--<code>Ativo</code>, <code>Inativo</code> ou <code>Baixado</code>.-->
                </td>
              </tr>
              <tr>
                 <td><strong>situacao_ie_desc</strong></td>
                 <td>string</td>
                 <td>Situação Cadastral da <strong>Inscrição Estadual</strong> (IE) no <strong>Sintegra</strong> sem tratamento. <br> 
                </td>
              </tr>
              <tr>
                 <td><strong>data_inicio_atividade</strong></td>
                 <td>string</td>
                 <td>Data do início da atividade no formato dd-MM-yyyy.</td>
              </tr>
              <tr>
                 <td><strong>regime_tributacao</strong></td>
                 <td>string</td>
                 <td>Regime de tributação.</td>
              </tr>
              <tr>
                 <td><strong>informacao_ie_como_destinatario</strong></td>
                 <td>string</td>
                 <td>Informação da Inscrição Estadual como destinatário.</td>
              </tr>
              <tr>
                 <td><strong>porte_empresa</strong></td>
                 <td>string</td>
                 <td>Porte da empresa.</td>
              </tr>
              <tr>
                 <td><strong>cnae_principal</strong></td>
                 <td>objeto</td>
                 <td>Atividade econômica principal.</td>
              </tr>
              <tr>
                 <td><strong>cnae_principal.code</strong></td>
                 <td>string</td>
                 <td>Código do CNAE principal</td>
              </tr>
              <tr>
                 <td><strong>cnae_principal.text</strong></td>
                 <td>string</td>
                 <td>Descrição da atividade econômica principal</td>
              </tr>
              <tr>
                 <td><strong>data_fim_atividade</strong></td>
                 <td>string</td>
                 <td>Data na qual a empresa foi cancelada no formato dd-MM-yyyy. <ins>Apenas para empresas com o status diferente de Ativo</ins>.</td>
              </tr>
              <tr>
                 <td><strong>uf</strong></td>
                 <td>string</td>
                 <td>Sigla da Unidade da Federação.</td>
              </tr>
              <tr>
                 <td><strong>cep</strong></td>
                 <td>string</td>
                 <td>CEP no formato 00000000.</td>
              </tr>
              <tr>
                 <td><strong>municipio</strong></td>
                 <td>string</td>
                 <td>Município.</td>
              </tr>
              <tr>
                 <td><strong>bairro</strong></td>
                 <td>string</td>
                 <td>Bairro.</td>
              </tr>
              <tr>
                 <td><strong>logradouro</strong></td>
                 <td>string</td>
                 <td>Logradouro.</td>
              </tr>
              <tr>
                 <td><strong>complemento</strong></td>
                 <td>string</td>
                 <td>Complemento.</td>
              </tr>
              <tr>
                 <td><strong>numero</strong></td>
                 <td>string</td>
                 <td>Número.</td>
              </tr>
              
              <tr>
                 <td><strong>ibge <span class="badge badge-pill glow" style="color: #ef678e;">novo</span></strong></td>
                 <td>objeto</td>
                 <td>IBGE.</td>
              </tr>
              <tr>
                 <td><strong>ibge.codigo_municipio</strong></td>
                 <td>string</td>
                 <td>Código IBGE do municipio.</td>
              </tr>
              <tr>
                 <td><strong>ibge.codigo_uf</strong></td>
                 <td>string</td>
                 <td>Código IBGE da UF.</td>
              </tr>

              <tr>
                 <td><strong>outras_ies <span class="badge badge-pill" style="color: #ef678e;">beta</span></strong></td>
                 <td>Array&lt;objeto&gt;</td>
                 <td>Retorna lista de outras <strong>inscrições estaduais.</strong> que o CNPJ tem.</td>
              </tr>
              <tr>
                 <td><strong>inscricao_estadual</strong></td>
                 <td>string</td>
                 <td>Inscrição Estadual.</td>
              </tr>
              <tr>
                 <td><strong>uf</strong></td>
                 <td>string</td>
                 <td>Sigla da Unidade da Federação.</td>
              </tr>
              <tr>
                 <td><strong>situacao_ie</strong></td>
                 <td>string</td>
                 <td>Situação Cadastral da <strong>Inscrição Estadual</strong> (IE) no <strong>Sintegra</strong>: <br> 
                  <strong style="color: #404040;">Valores possíveis</strong>:
                  <ul style="padding-left: 18px; padding-top: 10px;">
                    <li><code>Ativo</code></li>
                    <li><code>Inativo</code></li>
                    <li><code>Baixado</code></li>
                  </ul>
                 <!--<code>Ativo</code>, <code>Inativo</code> ou <code>Baixado</code>.-->
                </td>
              </tr>
			  <tr>
                 <td><strong>contribuinte_icms <span class="badge badge-pill" style="color: #ef678e;">beta</span></strong></td>
                 <td>Boolean</td>
                 <td>Verifica se a <strong>Inscrição Estadual</strong> (IE) no <strong>Sintegra</strong> é contribuinte de <strong>ICMS</strong>: <br> 
                  <strong style="color: #404040;">Valores possíveis</strong>:
                  <ul style="padding-left: 18px; padding-top: 10px;">
                    <li><code>True</code></li>
                    <li><code>False</code></li>
                  </ul>
                </td>
              </tr>
           </tbody>
        </table>
