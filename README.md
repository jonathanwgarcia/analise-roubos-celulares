# **Análise de Roubos e Furtos de Celulares no Rio de Janeiro entre 01/2014 e 09/2024**

A criminalidade envolvendo roubos e furtos de celulares tem se tornado uma preocupação crescente em muitas cidades do Brasil, especialmente no Rio de Janeiro. Com o aumento desses delitos, não apenas as vítimas enfrentam prejuízos materiais, mas também um impacto emocional e psicológico considerável.

Estudos recentes, como o levantamento do Datafolha encomendado pelo Fórum Brasileiro de Segurança Pública (FBSP), revelam que 9,2% da população brasileira foi vítima de furto ou roubo de celular. Este dado preocupa, especialmente considerando que 53% dos entrevistados evitam determinados locais ou horários por medo de serem vítimas desses crimes. No Rio de Janeiro, a situação é particularmente crítica, com mais de 10.574 celulares roubados bloqueados apenas através do programa Celular Seguro, que visa proteger os consumidores e desincentivar a revenda ilegal de aparelhos roubados.

Neste contexto, o presente projeto visa analisar dados relacionados a roubos e furtos de celulares no Rio de Janeiro, utilizando informações de roubos por bairro para identificar padrões e tendências de criminalidade. A partir dessa análise, buscamos oferecer insights valiosos para entender melhor a dinâmica dessa problemática crescente, que afeta tanto a segurança pública quanto o comportamento da população.

Este repositório contém uma análise exploratória de dados sobre roubos e furtos de celulares no município do Rio de Janeiro. A análise por bairros será feita através das Unidades territoriais, com base no CISP (número da circunscrição onde ocorreu o fato). A fonte dos dados é o [Instituto de Segurança Pública do Rio de Janeiro](http://www.ispdados.rj.gov.br/estatistica.html).

**Objetivos da Análise:**

* Identificar a tendência de roubos e furtos ao longo dos anos.
* Determinar quais bairros possuem o maior número de ocorrências de roubos e furtos.
* Analisar os meses com maior incidência de roubos e furtos.

  ![](http://wallpapercave.com/wp/cmdkr6o.jpg)

  # Dicionário de Referência

**Roubo**: Subtração de um bem com uso de violência ou ameaça à vítima. (Art. 157 do Código Penal Brasileiro)

**Furto**: Subtração de um bem sem uso de violência ou ameaça à vítima. (Art. 155 do Código Penal Brasileiro)

# Delegacias e Áreas Abrangidas

- **001a. Praça Mauá**: Centro (parte)
- **004a. Praça da República**: Centro (parte), Gamboa, Santo Cristo, Saúde
- **005a. Mem de Sá**: Centro (parte), Lapa, Paquetá
- **006a. Cidade Nova**: Catumbi, Cidade Nova, Estácio, Rio Comprido, Centro (parte)
- **007a. Santa Teresa**: Santa Teresa
- **009a. Catete**: Catete, Cosme Velho, Flamengo, Glória, Laranjeiras
- **010a. Botafogo**: Botafogo, Humaitá, Urca
- **011a. Rocinha**: Rocinha
- **012a. Copacabana**: Copacabana (parte), Leme
- **013a. Ipanema**: Copacabana (parte) *Apesar do nome, a DP fica localizada em Copacabana e abrange a parte do bairro próxima à Ipanema.
- **014a. Leblon**: Ipanema, Leblon
- **015a. Gávea**: Gávea, Jardim Botânico, Lagoa, São Conrado, Vidigal
- **016a. Barra da Tijuca**: Barra da Tijuca, Itanhangá, Joá
- **017a. São Cristóvão**: Caju, Mangueira, São Cristóvão, Vasco da Gama
- **018a. Praça da Bandeira**: Maracanã, Praça da Bandeira, Tijuca (parte)
- **019a. Tijuca**: Alto da Boa Vista, Tijuca (parte)
- **020a. Grajaú**: Andaraí, Grajaú, Vila Isabel
- **021a. Bonsucesso**: Benfica, Bonsucesso, Higienópolis, Manguinhos, Maré, Ramos
- **022a. Penha**: Brás de Pina (parte), Olaria, Penha, Penha Circular (parte)
- **023a. Méier**: Cachambi, Méier (parte), Todos os Santos (parte)
- **024a. Piedade**: Abolição, Água Santa (parte), Encantado, Engenho de Dentro (parte), Pilares, Piedade
- **025a. Engenho Novo**: Engenho Novo, Jacaré, Jacarezinho, Riachuelo, Rocha, Sampaio, São Francisco Xavier
- **026a. Todos os Santos**: Água Santa (parte), Engenho de Dentro (parte), Lins de Vasconcelos, Todos os Santos
- **027a. Vicente de Carvalho**: Colégio (parte), Irajá, Vicente de Carvalho, Vila Kosmos, Vila da Penha, Vista Alegre
- **028a. Praça Seca**: Vila Valqueire, Praça Seca, Tanque (parte)
- **029a. Madureira**: Cavalcanti, Engenheiro Leal, Madureira, Turiaçu, Vaz Lobo, Oswaldo Cruz (parte), Cascadura, Quintino Bocaiúva
- **030a. Marechal Hermes**: Bento Ribeiro, Campinho, Marechal Hermes, Oswaldo Cruz (parte)
- **031a. Ricardo de Albuquerque**: Anchieta, Guadalupe, Parque Anchieta, Ricardo de Albuquerque
- **032a. Taquara**: Anil, Cidade de Deus, Curicica, Gardênia Azul, Jacarepaguá, Taquara
- **033a. Realengo**: Campo dos Afonsos, Deodoro, Jardim Sulacap, Magalhães Bastos, Realengo, Vila Militar
- **034a. Bangu**: Bangu, Gericinó, Padre Miguel, Senador Camará
- **035a. Campo Grande**: Campo Grande, Cosmos, Inhoaíba, Santíssimo, Senador Vasconcelos
- **036a. Santa Cruz**: Paciência, Santa Cruz
- **037a. Ilha do Governador**: Bancários, Cacuia, Cidade Universitária, Cocotá, Freguesia, Galeão, Jardim Carioca, Jardim Guanabara, Moneró, Pitangueiras, Portuguesa, Praia da Bandeira, Ribeira, Tauá, Zumbi
- **038a. Braz de Pina**: Brás de Pina (parte), Cordovil, Jardim América, Parada de Lucas, Penha Circular (parte), Vigário Geral
- **039a. Pavuna**: Acari, Barros Filho, Costa Barros, Parque Colúmbia, Pavuna
- **040a. Honório Gurgel**: Coelho Neto, Colégio (parte), Honório Gurgel, Rocha Miranda
- **041. Tanque**: Freguesia (Jacarepaguá), Pechincha, Tanque (parte)
- **042a. Recreio**: Recreio dos Bandeirantes, Barra de Guaratiba, Camorim, Grumari, Vargem Grande, Vargem Pequena
- **043a. Pedra de Guaratiba**: Guaratiba, Pedra de Guaratiba, Sepetiba
- **044a. Inhaúma**: Del Castilho, Engenho da Rainha, Inhaúma, Maria da Graça, Tomás Coelho
