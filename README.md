# rodrigofranzoi.github.io

Site estático com a lista de aplicativos e os documentos legais de cada um (política de privacidade e termos de uso).

Site: [https://rodrigofranzoi.github.io](https://rodrigofranzoi.github.io)

Contato: [rodrigo.scroferneker@gmail.com](mailto:rodrigo.scroferneker@gmail.com)

## Apps

| App | Hub | Privacidade | Termos |
| --- | --- | --- | --- |
| Tabela TACO | [taco/](taco/index.html) | [privacy](taco/privacy.html) | [terms](taco/terms.html) |
| Tabela IBGE | [ibge/](ibge/index.html) | [privacy](ibge/privacy.html) | [terms](ibge/terms.html) |
| Loterias Brasil | [loterias/](loterias/index.html) | [privacy](loterias/privacy.html) | [terms](loterias/terms.html) |

URLs públicas (Loterias Brasil):

- https://rodrigofranzoi.github.io/loterias/privacy.html
- https://rodrigofranzoi.github.io/loterias/terms.html

`privacy.html` e `terms.html` na raiz redirecionam para a Tabela IBGE (links antigos).

## Estrutura

Cada app fica em uma pasta com o mesmo chrome (`style.css`):

```text
{slug}/
  index.html      hub (aviso + cards)
  privacy.html    PT (#politica-de-privacidade) e EN (#privacy-policy)
  terms.html      PT (#termos-e-condicoes) e EN (#terms-and-conditions)
```

## Incluir outro app

Copie `_templates/app/` e siga [.cursor/skills/add-app-legal/SKILL.md](.cursor/skills/add-app-legal/SKILL.md). Depois:

1. Preencha os placeholders e o conteúdo PT/EN.
2. Adicione o card em `index.html`.
3. Inclua a linha na tabela acima.
