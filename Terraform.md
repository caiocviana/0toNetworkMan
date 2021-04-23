### 🚀 Terraform
 Utilizaremos o Terraform para prover:
 
 - Criar uma nova instancia do GNS3 server;
 - Criar a infraestrutura para os estudos de AWS e GCP.
 
## Instalação
 
 Para essa instalação, utilizamos a [documentação](https://www.terraform.io/downloads.html) da HashiCorp.
 
## Instalação em Linux
 
 Faça o download do pacote:
 
 ```bash
 $ wget https://releases.hashicorp.com/terraform/0.15.0/terraform_0.15. 0_linux_amd64.zip
 ```
 
 Descompacte o pacote:
 
 ```bash
 $ unzip terraform_0.15.0_linux_amd64.zip
 ```
 
 Verifique os diretório utilizados na variavel $PATH. 
 
 ```bash
 $ echo $path
 ```
 
 Mova o diretório para um dos diretórios exibidos no comando anterior, abaixo um  exemplo:
 
 ```bash
 $ mv terraform /usr/local/bin/
 ```
 
 Verifique se a instalação foi realizada com sucesso:
 
 ```bash
 $ terraform -help
 ---
 Usage: terraform [global options] <subcommand> [args]
 
 The available commands for execution are listed below.
 The primary workflow commands are given first, followed by
 less common or more advanced commands.
 ```
 
 Para mais informações sobre instalação, [veja esta pagina da HashiCorp](https://learn.hashicorp.com/tutorials/terraform/install-cli?in=terraform/aws-get-started).