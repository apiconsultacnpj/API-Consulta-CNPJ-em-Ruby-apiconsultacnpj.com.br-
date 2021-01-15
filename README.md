# API Consulta CNPJ em Ruby (apiconsultacnpj.com.br)

### Consulta dados do CNPJ
```ruby
require 'faraday'

r = Faraday.get("https://api-publica.speedio.com.br/buscarcnpj?cnpj=00000000000191")
puts r.body
```

### Consulta quantas empresas tem no CEP
```ruby
require 'faraday'

r = Faraday.get("https://api-publica.speedio.com.br/buscar-atividade-location-distance?atividade=tecnologia&location=01009-907&distance=5")
puts r.body
```

### Consulta a idade média do setor
```ruby
require 'faraday'

r = Faraday.get("https://api-publica.speedio.com.br/buscar-atividade-idade-media?atividade=mercado&location=SP")
puts r.body
```


