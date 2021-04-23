# GNS3 Server

Utilizamos o GNS3 server para criação dos laboratórios. Dentro dele, conseguimos montar as topologias, inserindo servidores, switches, roteadores e firewalls.

Para mais informações sobre o [GNS3](https://www.gns3.com/).

---

## Instalação e Configuração

Para instalação do GNS3 server, utilizaremos uma imagem do ubuntu server e a [documentação da própria GNS3](https://docs.gns3.com/docs/getting-started/installation/linux). Porém pode ser feita com outras distribuições e com outros sistemas operacionais.

Após a instalação, acessamos via ssh a EC2 e adicionamos algumas configurações no arquivo gns3-server.conf (Caso não exista, você pode cria-lo) para ignorar os alarmes referentes ao suporte KVM. 

Arquivo:

```bash
sudo vi ~/.config/GNS3/2.2/gns3_server.conf
```

Insira as linhas abaixo no arquivo:

```bash
[Qemu]
enable_hardware_acceleration = false
require_hardware_acceleration = false
enable_kvm = false
```

Inicie o gns3server

```bash
gns3server
```

Acesse no browser o endereço da sua instancia na porta 3080:

```bash
http://ec2-ip:3080/
```