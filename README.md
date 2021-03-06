# IBGE

A <a title="Link da API" href="https://servicodados.ibge.gov.br" target="_blank">**_API do IBGE_**</a> possibilita baixar os dados diretamente para o _script_. Para baixar as malhas, ou seja, informações geoespaciais, é possivel baixar os dados em três diferentes formatos:
- **_?formato=application/vnd.geo+json_**, para baixar os dados em GeoJson;
- **_?formato=application/json_**, para baixar os dados em TopoJson;
- **_?formato=image/svg+xml_**, para baixar os dados em SVG;

É possível definir a resolução que, na prática, refere-se ao nível de detalhamento do dado obtido.
- **_?resolucao=0_**, Nenhuma divisão político-administrativa é inserida no interior da malha
- **_?resolucao=1_**, Inclui na malha as macrorregiões. Válido apenas quando a localidade for BR.
- **_?resolucao=2_**, Inclui na malha as Unidades da Federação. Válido apenas quando a localidade for BR ou uma macroregião
- **_?resolucao=3_**, inclui na malha as mesorregiões. Válido apenas quando a localidade for BR, macroregião ou Unidade da Federação
- **_?resolucao=4_**, Inclui na malha as microrregiões. Válido apenas quando a localidade for BR, macroregião, Unidade da Federação ou mesorregião
- **_?resolucao=5_**, inclui na malha os municípios

E a qualidade.
- **_?qualidade=1_**, pior qualidade;
- **_?qualidade=2_**, razoável qualidade;
- **_?qualidade=3_**, boa qualidade;
- **_?qualidade=4_**, melhor qualidade;


{: .alert .alert-danger}
**Aviso:** Esse _post_ tem a finalidade de mostrar os comandos básicos e me deixar com uma "cola" rápida para meu uso cotidiano. Todas os códigos são exemplificativos e podem/devem ser alterados, indicando o nome dos arquivos e diretórios corretamente.

{: .box-note}
**Nota:** É possível acessar esse _post_ em formato <a title="Link do Folium" href="https://github.com/michelmetran/api_ibge/raw/master/docs/api_ibge.pdf" target="_blank">**_pdf_**</a>, diretamente por meio do <a title="Link do Repositório" href="https://github.com/michelmetran/api_ibge" target="_blank">**repositório do GitHub**</a> ou ainda, de maneira interativa, usando o [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/michelmetran/api_ibge/master).

