---


---

<h1 id="api-rest">API-REST</h1>
<p>O objetivo da Integração API da Yandeh é permitir que o lojista continue utilizando sua solução de frente de caixa (Automação Comercial ou PDV) e a integre através de uma API construída no padrão REST</p>
<p>A API Yandeh possui as seguintes características:</p>
<p>• Recursos REST, de forma que seja possível acessar por meio de semântica HTTP padrão.</p>
<p>• Códigos de status HTTP para comunicar o sucesso/erro nas chamadas.</p>
<p>• Todas as requisições e respostas encontram-se no formato JSON.</p>
<blockquote>
<p>Acesse a documentação <a href="https://app.swaggerhub.com/apis/thiago.franca/erp-yandeh-integration/1.0.0.8/">Swagger Hub</a>.</p>
</blockquote>
<h1 id="linguagem-de-programação">Linguagem de Programação</h1>
<p>A solução <strong>API Rest</strong> da plataforma <strong>da Yandeh Integration</strong> foi desenvolvida com a tecnologia REST, que é padrão de mercado e independe da tecnologia utilizada por nossos clientes. Dessa forma, é possível integrar-se utilizando as mais variadas linguagens de programação, tais como:</p>
<ul>
<li>
<p>ASP</p>
</li>
<li>
<p>Net</p>
</li>
<li>
<p>Java</p>
</li>
<li>
<p>PHP</p>
</li>
<li>
<p>Ruby</p>
</li>
<li>
<p>Python</p>
</li>
</ul>
<h2 id="segurança">Segurança</h2>
<p>Estas operações devem ser executadas utilizando sua chave específica que chamamos de <strong>TOKEN</strong>, o mesmo será responsável por autenticar o acesso ao sistema.</p>
<blockquote>
<p><strong>Note:</strong> Solicitar acesso para equipe integração da Yandeh.</p>
</blockquote>
<h2 id="certificado-ssl">Certificado SSL</h2>
<p>O Certificado SSL para servidor web oferece autenticidade e integridade dos dados de um web site, proporcionando aos clientes das lojas virtuais a garantia de que estão realmente acessando o site que desejam, e não uma um site fraudador.</p>
<h2 id="glossário-dos-métodos">Glossário dos Métodos</h2>
<p>A troca de mensagens são pelas URLs  os métodos receberão as mensagens HTTP através dos métodos POST, GET ou PUT.</p>

<table>
<thead>
<tr>
<th>Método</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>POST</strong></td>
<td><code>'Envio de informações que serão processadas. Por exemplo, criação de uma transação'</code></td>
</tr>
<tr>
<td><strong>PUT</strong></td>
<td><code>"Utilizado para atualização de um recurso já existente. Por exemplo, captura ou cancelamento de uma transação previamente autorizada."</code></td>
</tr>
<tr>
<td><strong>GET</strong></td>
<td><code>Utilizado para consultas de recursos já existentes. Por exemplo, consulta de transações.</code></td>
</tr>
</tbody>
</table>
