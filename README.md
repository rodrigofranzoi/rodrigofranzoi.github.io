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
| Nutri Rótulo | [nutri-rotulo/](nutri-rotulo/index.html) | [privacy](nutri-rotulo/privacy.html) | [terms](nutri-rotulo/terms.html) |
| DiningXP | [diningxp/](diningxp/index.html) | [privacy](diningxp/privacy.html) | [terms](diningxp/terms.html) |
| Clipboard Buddy | [clipboard-buddy/](clipboard-buddy/index.html) | [privacy](clipboard-buddy/privacy.html) | [terms](clipboard-buddy/terms.html) |
| Screenshot Buddy | [screenshot-buddy/](screenshot-buddy/index.html) | [privacy](screenshot-buddy/privacy.html) | [terms](screenshot-buddy/terms.html) |
| OTP Buddy | [otp-buddy/](otp-buddy/index.html) | [privacy](otp-buddy/privacy.html) | [terms](otp-buddy/terms.html) |

URLs públicas (Buddy — macOS):

- https://rodrigofranzoi.github.io/clipboard-buddy/privacy.html
- https://rodrigofranzoi.github.io/clipboard-buddy/terms.html
- https://rodrigofranzoi.github.io/screenshot-buddy/privacy.html
- https://rodrigofranzoi.github.io/screenshot-buddy/terms.html
- https://rodrigofranzoi.github.io/otp-buddy/privacy.html
- https://rodrigofranzoi.github.io/otp-buddy/terms.html

URLs públicas (DiningXP):

- https://rodrigofranzoi.github.io/diningxp/privacy.html
- https://rodrigofranzoi.github.io/diningxp/terms.html
- Fonte oficial do benefício (American Express França): https://www.americanexpress.com/fr-fr/benefits/diningbenefit

`privacy.html` e `terms.html` na raiz redirecionam para a Tabela IBGE (links antigos).

## Estrutura

Cada app fica em uma pasta com o mesmo chrome (`style.css`):

```text
{slug}/
  index.html      hub (aviso + cards)
  privacy.html    PT / EN / FR (#politica-de-privacidade, #privacy-policy, #politique-de-confidentialite)
  terms.html      PT / EN / FR (#termos-e-condicoes, #terms-and-conditions, #conditions-d-utilisation)
                  (DiningXP inclut le français ; les autres apps restent PT+EN)
```

## Incluir outro app

Copie `_templates/app/` e siga [.cursor/skills/add-app-legal/SKILL.md](.cursor/skills/add-app-legal/SKILL.md). Depois:

1. Preencha os placeholders e o conteúdo PT/EN.
2. Adicione o card em `index.html`.
3. Inclua a linha na tabela acima.
