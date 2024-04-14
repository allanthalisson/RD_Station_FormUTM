# Tracking UTMs no RD Station Form
Este projeto apresenta uma solução para a falta de visibilidade de informações de campanhas nos cards dos leads dentro do RD Station Marketing.

## Instruções

## 1. Criando os campos de UTMs
A primeira coisa que você precisará fazer é criar os campos personalizados no RD Station. No menu Converter > Campos Personalizados você precisará criar os campos: utm_source, utm_medium, utm_campaign e utm_content. *Lembre-se de manter a nomenclatura conforme descrito aqui.*

*_Exemplo de configuração:_*

> Nome do campo: utm_campaign
> 
> Enunciado do campo: utm_campaign
> 
> Tipo de campo: Campo aberto - Texto

## 2. Inserindo os campos no formulário
Após criar os campos, insira-os no formulário e, por enquanto, não se preocupe se eles ficarão visíveis.

## 3. Inserindo os campos no formulário
Copie o códido em [Form RD](https://github.com/allanthalisson/tracking_utm/blob/f3a8e1b21fc3af1ae67ab0ffa80dd61fb2509714/form_RD).

Com o código copiado, vá até as configurações de sua Landing Page no RD Station e acesse a opção de Edição Avançada, inserindo o código na aba *"Javascript em HEAD"*.

![image](https://github.com/allanthalisson/tracking_utm/assets/166962056/3b042e6d-f607-488d-a3e8-d92bb48151ae)

Salve todas as alterações e publique a Landing Page.

## 4. Testando o script
Acesse a url de sua landing page inserindo alguns caracteres de utm como teste. Por exemplo: https://suapagina/?utm_source=google&utm_medium=cpc&utm_campaign=campanha_01&utm_content=ad_01

Após a página ser carregada, confira se os campos de utm do formúlario estão ocultos. Abra o console de navegador (Ctrl + Shft + I), vá até a aba Console e cole o código presente em [Console Verify](https://github.com/allanthalisson/tracking_utm/blob/f3a8e1b21fc3af1ae67ab0ffa80dd61fb2509714/console_verify). Após colar o código, aperte enter.

O console deverá retornar algo do tipo:

![Imagem do WhatsApp de 2024-04-13 à(s) 20 11 38_d316a9d1](https://github.com/allanthalisson/tracking_utm/assets/166962056/4b7cb58c-3cfc-4d75-9b83-5e0a0e280c3b)

*Isso significa que nosso código funcionou!* Agora preencha os campos do formulário e envie-o. Confira se as informações chegaram corretamente na sua base de leads do RD Station.
