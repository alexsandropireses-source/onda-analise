# Onda Analise

Site estático de previsão de ondas e vento para esportes aquáticos no Brasil.

## Publicação

O site é publicado pelo GitHub Pages. O workflow em `.github/workflows/pages.yml` publica automaticamente a cada envio para a branch `main`.

## Dados da previsão

- Ondas e ondulação: modelo NOAA/NCEP GFS-Wave, consultado pela API Marine do Open-Meteo.
- Vento e rajadas: modelo NOAA GFS, consultado pela API GFS do Open-Meteo.
- Nível do mar: estimativa horária com efeito da maré e outros fatores oceânicos.

A página consulta os modelos ao vivo quando uma região é selecionada. A análise compara horários de cada dia, explica altura, período, vento e direção da ondulação em linguagem simples e mostra uma nota indicativa — não uma garantia de condições ou segurança.

A altura do nível do mar é relativa ao nível médio global e pode diferir da tábua de maré local. A precisão dos modelos pode ser limitada perto da costa; confira as condições locais.

## Regiões

Os estados aparecem no seletor. As praias e regiões cadastradas estão em `spots.js`, com coordenadas aproximadas. Para incluir um pico, adicione um item ao array `MARE_SPOTS`.

## Atribuição

Dados via Open-Meteo, com atribuição ao DWD. Consulte os [termos e atribuição do Open-Meteo](https://open-meteo.com/en/terms) antes de uso comercial.
