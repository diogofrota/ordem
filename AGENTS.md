# Instruções para o Codex — Projeto Ordena

## 1. REGRA PRINCIPAL: NÃO APAGAR CÓDIGO

- Nunca excluir código existente do projeto.
- Nunca remover funções, componentes, elementos HTML, JavaScript, CSS ou trechos de código existentes sem autorização explícita do usuário.
- Quando um trecho existente deixar de ser utilizado, NÃO deletar.
- Comentar o trecho antigo e mantê-lo no arquivo.

Exemplo:

Antes:

<div class="old-card">
  ...
</div>

Se não for mais utilizado:

<!--
<div class="old-card">
  ...
</div>
-->

Para JavaScript:

// Código antigo mantido por segurança
// function exemploAntigo() {
//   ...
// }

Sempre priorizar preservar o código original.

---

## 2. ALTERAÇÕES DEVEM SER INCREMENTAIS

- Aproveitar o código existente sempre que possível.
- Evitar reescrever arquivos inteiros.
- Alterar somente o necessário para cumprir a tarefa solicitada.
- Novas funcionalidades podem ser adicionadas normalmente.
- Não realizar refatorações gerais sem solicitação explícita.
- Não reorganizar código apenas por estética.
- Não alterar partes não relacionadas à tarefa atual.

---

## 3. TRABALHAR SOMENTE NA PÁGINA SOLICITADA

IMPORTANTE:

Por padrão, cada tarefa deve modificar SOMENTE a página indicada pelo usuário.

Não alterar outras páginas, arquivos ou componentes, exceto quando for estritamente necessário para o funcionamento da página solicitada.

Antes de modificar qualquer outro arquivo além da página solicitada, verificar se realmente é necessário.

Não realizar alterações globais no projeto sem solicitação explícita.

Esta regra poderá ser removida futuramente quando o projeto passar para uma fase de alterações gerais.

---

## 4. MANTER O PADRÃO VISUAL EXISTENTE

Ao criar ou modificar páginas:

- Utilizar o mesmo padrão visual já existente no projeto.
- Manter as mesmas fontes.
- Manter os mesmos tamanhos de fonte.
- Manter espaçamentos semelhantes.
- Manter padrão de cards.
- Manter padrão de botões.
- Manter padrão de tabelas.
- Manter padrão de cabeçalhos.
- Manter padrão de cores.
- Manter padrão de responsividade.
- Manter as classes Bootstrap já utilizadas pelo projeto.

Não criar um novo padrão visual se já existir um componente equivalente no projeto.

---

## 5. FORMULÁRIOS

Existe no projeto uma pasta/página de referência contendo exemplos de formulários.

Antes de criar qualquer formulário novo:

1. Localizar os formulários existentes no projeto.
2. Analisar o padrão utilizado.
3. Reutilizar esse padrão.

Utilizar como referência os componentes existentes para:

- campos de texto;
- select;
- textarea;
- checkbox;
- radio button;
- data;
- hora;
- calendário/date picker;
- upload de arquivos;
- switches;
- validações;
- labels;
- mensagens de erro;
- botões de salvar/cancelar.

Não criar componentes de formulário com aparência diferente se já existir um exemplo equivalente no projeto.

Se existir um componente pronto, preferir reutilizá-lo ou copiar sua estrutura.

---

## 6. CRIAÇÃO DE NOVAS PÁGINAS

Ao criar uma nova página:

- Usar uma página existente semelhante como referência.
- Manter a mesma estrutura do projeto.
- Manter header, sidebar, footer, breadcrumbs e containers existentes.
- Manter o mesmo padrão Bootstrap.
- Manter o mesmo padrão de CSS e JavaScript.
- Não criar bibliotecas novas se a funcionalidade já puder ser feita com as bibliotecas existentes.

A nova página deve parecer parte natural do sistema existente.

---

## 7. REUTILIZAÇÃO

Antes de criar código novo:

- procurar componentes semelhantes;
- procurar formulários semelhantes;
- procurar funções JavaScript existentes;
- procurar CSS existente;
- procurar componentes Bootstrap já utilizados.

Preferir reutilização em vez de duplicação.

---

## 8. BIBLIOTECAS E DEPENDÊNCIAS

- Não adicionar novas bibliotecas sem necessidade.
- Não trocar versões de bibliotecas existentes sem autorização.
- Não remover bibliotecas existentes.
- Utilizar preferencialmente os recursos já presentes no projeto.

---

## 9. RESPONSIVIDADE

Todas as alterações devem respeitar o padrão responsivo existente.

Priorizar:

- mobile first;
- Bootstrap grid;
- comportamento adequado em celular;
- tablet;
- desktop.

Não quebrar layouts existentes.

---

## 10. ESCOPO DA TAREFA

Quando o usuário disser, por exemplo:

"Trabalhe na página cadastro-viaturas.html"

O escopo padrão será:

cadastro-viaturas.html

O Codex deve concentrar as alterações nessa página.

Arquivos externos como CSS ou JavaScript somente devem ser modificados quando forem realmente necessários para essa página.

Não aproveitar a tarefa para corrigir ou modificar outras partes do sistema.

---

## 11. ANTES DE ALTERAR

Antes de implementar uma mudança:

1. Ler a página solicitada.
2. Identificar componentes semelhantes no projeto.
3. Verificar a pasta/página de formulários de referência.
4. Identificar o padrão visual existente.
5. Implementar seguindo esse padrão.

---

## 12. PRESERVAÇÃO É PRIORIDADE

Em caso de dúvida entre:

- remover código;
- ou preservar código;

sempre PRESERVAR.

Em caso de substituição de uma solução existente:

- comentar a implementação antiga;
- inserir a nova implementação;
- deixar claro através de comentário qual trecho foi substituído.

Nunca destruir código existente silenciosamente.

## REFERÊNCIA OBRIGATÓRIA DE FORMULÁRIOS

A pasta:

pages/forms/

é a referência visual e estrutural oficial para formulários do projeto.

Antes de criar campos de formulário em qualquer página, consultar os exemplos existentes nessa pasta.

Se precisar criar:

- calendário → procurar primeiro exemplo de calendário;
- checkbox → procurar primeiro exemplo de checkbox;
- select → procurar primeiro exemplo de select;
- data → procurar primeiro exemplo de campo de data;
- upload → procurar primeiro exemplo de upload.

Copiar/adaptar o padrão existente em vez de criar um componente visual novo.

## Feedback visual obrigatório para operações

Todas as páginas e funcionalidades do projeto devem fornecer feedback visual ao usuário durante operações assíncronas, principalmente operações relacionadas a API e banco de dados.

Esta regra deve ser aplicada em novos desenvolvimentos e, quando uma página existente for alterada, deve ser incorporada sem remover funcionalidades ou código existente.

### Regra de preservação

- Nunca apagar código existente sem necessidade.
- Nunca remover funcionalidades existentes.
- Caso um trecho deixe de ser utilizado, preferir comentá-lo em vez de apagá-lo.
- As alterações devem ser incrementais.
- Manter o padrão visual e estrutural já existente no projeto.
- Antes de criar novos componentes, verificar se existe componente/padrão equivalente no próprio projeto e reutilizá-lo.

### Loading

Sempre que houver comunicação assíncrona, incluindo:

- carregamento inicial da página;
- busca de registros;
- consulta ao banco de dados;
- envio de formulário;
- cadastro;
- edição;
- atualização;
- exclusão;
- ativação/desativação;
- qualquer operação que dependa de API ou banco;

deve existir uma indicação visual de processamento.

Preferencialmente reutilizar o componente de loading "Growing Dots" já definido no projeto.

O loading deve:

- aparecer imediatamente após o início da operação;
- permanecer visível enquanto a operação estiver em andamento;
- desaparecer somente após conclusão ou erro;
- nunca permanecer ativo indefinidamente após uma falha.

Quando a página depender de vários dados para sua renderização completa, manter o loading até que todos os dados obrigatórios tenham sido recebidos e tratados.

### Botões durante operações

Quando uma operação for iniciada através de um botão:

- desabilitar temporariamente o botão para impedir múltiplos envios;
- mostrar um spinner/loading quando apropriado;
- alterar temporariamente o texto para indicar a operação, como:
  - Salvando...
  - Cadastrando...
  - Atualizando...
  - Excluindo...
  - Carregando...
- restaurar o botão após conclusão ou erro.

### Mensagens de sucesso

Toda operação concluída com sucesso deve gerar uma confirmação visual clara.

Utilizar o padrão de alertas já existente no projeto, preferencialmente Bootstrap `alert-success`, com ícone de confirmação quando compatível com a página.

Exemplos:

- "Viatura cadastrada com sucesso."
- "Ponto de baseamento cadastrado com sucesso."
- "Registro atualizado com sucesso."
- "Registro excluído com sucesso."
- "Dados salvos com sucesso."

O estilo deve seguir como referência os alertas de sucesso já existentes, como o utilizado no cadastro de Pontos de Baseamento.

### Mensagens de erro

Toda operação que falhar deve gerar feedback visual.

Ao ocorrer erro:

- remover o loading;
- reabilitar botões e controles;
- informar claramente que a operação não foi concluída;
- não limpar dados preenchidos desnecessariamente;
- permitir que o usuário tente novamente.

Exemplos:

- "Não foi possível concluir a operação."
- "Erro ao carregar os dados."
- "Não foi possível salvar as informações. Tente novamente."

### Princípio geral

Nenhuma operação relevante deve acontecer silenciosamente.

O usuário deve sempre conseguir perceber visualmente:

1. que a operação começou;
2. que está sendo processada;
3. que terminou com sucesso;
4. ou que ocorreu um erro.