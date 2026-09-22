# AGENTS.md

É um arquivo de instruções usado para orientar agentes de codificação de IA.

Pense em AGENTS.md como um README para agentes: um lugar dedicado e previsível fornecer contexto e instruções para ajudar agentes de codificação de IA a trabalharem no seu projeto.

Abaixo está um exemplo mínimo de arquivo AGENTS.md:

```markdown
# Instruções gerais apenas para desenvolvimento Delphi
- Adicione sempre uma `uses` por linha
- Adicione as units sempre na cláusula `uses` da interface e nunca na implementation
- Sempre que uma nova unit for criada para ser usada no projeto, ela deve ser adicionada aos arquivos `.dpr` e `.dproj`
- Ao chamar um método local, use sempre `Self.`. Por exemplo, se o método declarado tem o nome `Clear`, ao chamá-lo na mesma classe use `Self.Clear`. Mas não faça isso para componentes se o nome do TButton é `btnGravar` chame 'btnGravar.Click' e não 'Self.btnGravar.Click'
## Prefixo para componentes
| Componente | Prefixo | Exemplo |
| TLabel | lb | lbNome |
| TEdit | edt | edtNome |
| TDateTimePicker | edt | edtDataIni |
| TDBEdit | lb | lbNome |
| TButton | btn | btnGravar |

## Ignorar completamente
.git\
dcu\
__history/
__recovery/
*.~*

## Cuidados ao editar arquivos .dfm/.fmx
- Nunca use acentos ou caracteres não ASCII nos nomes de componentes. Exemplo: use `ckComposicao`, não `ckComposição`.
- Ao editar strings com acentos em `.dfm`/`.fmx`, use escapes Delphi completos e válidos, mantendo a aspa final. Exemplo correto: `Caption = 'Tipo opera'#231#227'o'`.
- Após editar `.dfm`/`.fmx`, valide o arquivo com o conversor do RAD Studio antes de finalizar, preferencialmente em uma cópia temporária: `convert.exe -i Caminho\Arquivo.dfm`.

# Idioma
- Responda sempre em português do Brasil (pt-BR).

```

## Os arquivos AGENTS.md podem ficar nos seguintes níveis:

### 1. Global
Regras pessoais aplicadas a todos os projetos
```
C:\Users\SEU_USUARIO\.codex\AGENTS.md
```

```
%USERPROFILE%\.codex\AGENTS.md
```

### 2. Raiz do projeto
Regras gerais do projeto / repositório
```
C:\Projeto\AGENTS.md
```

### 3. Subdiretórios
Regras específicas do módulo. Quanto mais próximo do código, maior a prioridade

```
C:\Projeto\Modulo\AGENTS.md
```


## 📞 Contatos
[![Telegram](https://img.shields.io/badge/Telegram-Join-blue?logo=telegram)](https://t.me/Code4Delphi)
[![YouTube](https://img.shields.io/badge/YouTube-Join-red?logo=youtube&logoColor=red)](https://www.youtube.com/@code4delphi)
[![Instagram](https://img.shields.io/badge/Intagram-Follow-red?logo=instagram&logoColor=pink)](https://www.instagram.com/code4delphi/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/cesar-cardoso-dev)
[![Blog](https://img.shields.io/badge/Blog-Code4Delphi-F00?logo=delphi)](https://code4delphi.com.br/blog/)
[![Course](https://img.shields.io/badge/Course-Delphi-F00?logo=delphi)](https://code4delphi.github.io/ia-devs-delphi-lazarus/)
[![E-mail](https://img.shields.io/badge/E--mail-Send-yellowgreen?logo=maildotru&logoColor=yellowgreen)](mailto:contato@code4delphi.com.br)
