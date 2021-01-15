# API Consulta CNPJ em Ruby (apiconsultacnpj.com.br)

### Consultar dados de um determinado CNPJ
```ruby
require 'net/http'
require 'uri'

uri = URI.parse("https://api-publica.speedio.com.br/buscarcnpj?cnpj=00000000000191")
r = Net::HTTP.get_response(uri)
puts r.body
```

### Consultar quantas empresas existem em um determinado CEP
```ruby
require 'net/http'
require 'uri'

uri = URI.parse("https://api-publica.speedio.com.br/buscar-atividade-location-distance?atividade=tecnologia&location=01009-907&distance=5")
r = Net::HTTP.get_response(uri)
puts r.body
```

### Consultar a idade média de vida de um determinado setor
```ruby
require 'net/http'
require 'uri'

uri = URI.parse("https://api-publica.speedio.com.br/buscar-atividade-idade-media?atividade=mercado&location=SP")
r = Net::HTTP.get_response(uri)
puts r.body
```
