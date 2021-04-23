# ☁️ AWS CLI
 Este pacote da AWS terá duas funções:
 
 - Exibir/Executar configurações na Cloud;
 - Aproveitar as credencias para executar o código do Terraform.
 
 Seguiremos a [documentação](https://docs.aws.amazon.com/pt_br/cli/latest/userguide/install-cliv2.html) para instalação.

## Pré Requisitos
 - Usuário de serviço com permissão
 
## Instalação em Linux

 Para demais sistemas operacionais, utilizem a documentação mencionada acima.

```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

## Configuração
 Execute o comando "aws configure" após a instalação. Abaixo um **exemplo** de configuração com  os valores.
 **Importante:** Tenha um usuário de serviços criado na AWS sem permissão de acesso via console (web).

 ```markdown
 aws configure
 AWS Access Key ID [None]: AKIAIOSFODNN7EXAMPLE
 AWS Secret Access Key [None]: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
 Default region name [None]: sa-east-1
 Default output format [None]: json
 ```
 
 Para mais [informações](https://docs.aws.amazon.com/pt_br/cli/latest/userguide/cli-configure-quickstart.html) sobre configurações.

