---
title: "Instalação / Download"
summary: Como baixar e rodar a ferramenta Market2csv
date: 2025-04-25T23:08:11-03:00
aliases: [instalacao/download]
draft: false
---

### **Não é necessário instalação da ferramenta. Basta baixar a ferramente e rodar**

<!-- Você pode baixar diretamente do link do projeto no github (não precisa ter conta no site para baixar os arquivos) -->

\>\>\> **BAIXE A FERRAMENTA SOMENTE DO LINK DO PROJETO NO GITHUB** \<\<\<

-> Link do projeto no github ([market2csv](https://github.com/caiowirthmann/market2csv))
^ alterar para link da release
^ indicar qual versão baixar dependendo do sistema (`.exe` para windows, `.bin` para unix)

---

### Executando a ferramenta no Windows

1. Baixe o arquivo `.exe` ou extraia a ferramenta da pasta compactada `.zip` e salve na pasta onde quer que os arquivos das extrações sejam salvas

2. Execute a ferramenta (pode ser que você tenha que dar permissão para executar como administrador, dependendo de como esteja configurado seu computador)

3. As pastas `extracoes` e `logs` onde são gerados os arquivos são criados na mesma pasta onde o executável do `market2csv` está salvo

*Para dar permissão de administrador, basta clicar com o botão direito no arquivo e clicar na opção "executar como administrador". Ou se quiser tornar essa opção padrão para esse arquivo, clique em **Propriedades >> Atalho >> Avançado >> Executar como administrador** e depois clicar em OK*


---

### Executando a ferramenta em sistemas Unix (linux, macOs)

1. Baixe o arquivo `binário` ou extraia a ferramenta da pasta compactada `.tar.gz` e salve na pasta onde quer que os arquivos das extrações sejam salvas

```bash
# criando a pasta onde irá salvar a ferramenta
mkdir -p market2csv

# extraindo o .tar.gz para a pasta market2csv
tar -xzvf market2csv-linux.v1.0.0.tar.gz -C market2csv
```

2. De permissão e execute o arquivo

```bash
sudo chmod +x market2csv-linux
./market2csv-linux
```

Caso queira, você pode criar um `alias` para executar a ferramenta de qualquer lugar, basta entrar no seu `.bashrc` e adicionar a seguinte linha

*Substitua o nome do alias e o caminho onde a ferramenta está salva para o seu caso*
```bash
alias market2csv='~/home/market2csv/market2csv-linux'
```

3. As pastas `extracoes` e `logs` onde são gerados os arquivos são criados na mesma pasta onde o binário do `market2csv` está salvo

---


### Executando a ferramenta diretamente pelo código-fonte

Requisitos:
- Go `+1.24.0` instalado ([Caso não tenha, siga as instruções aqui](https://golang.org/doc/install))
- Git instalado ([Caso não tenha siga as intruções aqui](https://git-scm.com/))

##### Clone o repositório do github

```bash
git clone https://github.com/caiowirthmann/market2csv.git
cd market2csv
```

#### Executando a ferramenta


```go
// executando a ferramenta diretamente pelo código fonte
go run main.go
```

#### Compilando a ferramenta

1. Compile a ferramenta
```go
go build -o market2csv
```

2. De a permissão e execute a ferramenta 
```bash
sudo chmod +x market2csv
./market2csv
```