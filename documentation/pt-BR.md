<!-- ELUCENIA technical documentation · spesi · pt-BR · no clinical/professional/rights approval -->

# sPESI (PESI simplificado)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/spesi)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Idade \> 80 anos

`idade`

### Câncer (ativo ou tratado no último ano)

`cancer`

### Doença cardiopulmonar crônica (insuficiência cardíaca ou doença pulmonar crônica)

`cardiopulm`

### FC ≥ 110 bpm

`fc`

### PA sistólica \< 100 mmHg

`pas`

### SatO₂ \< 90%

`sat`

## Edição do método

s PESI/Jimenez 2010:6 variáveisbinárias,0 baixoriscorestantealto; sem PESIoriginal 11 variáveis

## Fórmula documentada

Um ponto para cada item: idade \> 80, câncer, doença cardiopulmonar crônica, FC ≥ 110, PAS \< 100 e SatO₂ \< 90%. Zero ponto = baixo risco; ≥ 1 ponto = alto risco pelo sPESI.

## Limites e população

sPESI estima prognóstico em TEP agudo, não confirma nem exclui TEP. Baixo risco no estudo ainda apresentou mortes e não representa autorização isolada de tratamento ambulatorial. Instabilidade, comorbidades, fatores clínicos e condições logísticas devem ser avaliados no protocolo correspondente.

## Referências

- [Jiménez D et al. Simplification of the pulmonary embolism severity index for prognostication in patients with acute symptomatic pulmonary embolism. Arch Intern Med, 2010.](https://doi.org/10.1001/archinternmed.2010.199)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism developed in collaboration with the European Respiratory Society (ERS). Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Baixo risco: mortalidade em 30 dias de 1,0%

Candidato a alta precoce ou tratamento domiciliar, se não houver outros impeditivos (critérios de Hestia).


### 2

Não é baixo risco: mortalidade em 30 dias de 10,9%

Risco intermediário pela ESC: avaliar ventrículo direito (eco ou angiotomografia) e troponina.


### 3

Não é baixo risco: mortalidade em 30 dias de 10,9%

Risco intermediário pela ESC: avaliar ventrículo direito (eco ou angiotomografia) e troponina.

