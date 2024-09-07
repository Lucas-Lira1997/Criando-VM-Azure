# **Criando-VM-Azure**
Guia para criação de máquina virtual (VM) utilizando o Microsoft Azure

## 1. **Primeiros Passos**
- Após o cadastro no site [Microsoft Azure](https://azure.microsoft.com/pt-br/pricing/purchase-options/azure-account), iremos pesquisar na barra de pesquisa por *máquinas virtuais*.
- Quando selecionamos a opção _**Criar**_, no canto superior esquerdo, mostrará 3 opções para criar sua máquina virtual. Para fins didaticos, iremos selecionar a opção _**Máquina virtual do azure**_.
## 2. **Detalhes do projeto**
Aqui iremos escolher a assinatura adotada para gerenciar os custos e os recursos aplicados na sua máquina virtual. Iremos também, definir o grupo de recursos que queremos criar para deixarmos organizados em pastas, organizando os recursos aplicados.
- A assinatura deixaremos a que já está pré-selecionda _**Azure subscription 1**_.
- No grupo de recursos, podem escolher qualquer nome para sua pasta.
## 3. **Detalhes da instância**
- Primeiramente, escolhemos um _**nome para nossa máquina virtual**_. Importante destacar que as máquinas virtuais do Azure possuem dois nomes distintos: o nome da máquina virtual usado como identificador de recursos e o nome do host do convidado. Automaticamente, ao definirmos o nome da máquina virtual o Azure atribui o mesmo nome para o host, podendo alterar somente o nome do host quando entrar na máquina virtual. Vale salientar que o _**nome da máquina virtual não pode ser alterado após a criação da VM**_.
- Logo em seguida, _**escolhe-se a região**_ ideal para você. Nem todos os tamanhos de VM's estão disponíveis para todas as regiões.
- Nas opções de disponibilidade, podemos escolher como será o gerenciamento e a resiliência para os aplicativos. O Azure oferece 3 opções: [Zonas de disponibilidade](https://learn.microsoft.com/pt-br/azure/virtual-machines/availability#availability-zones), [Conjuntos de dimensionamento de máquinas virtuais](https://learn.microsoft.com/pt-br/azure/virtual-machines/availability#virtual-machines-scale-sets) e [Conjuntos de disponibilidade](https://learn.microsoft.com/pt-br/azure/virtual-machines/availability#availability-sets).
- Quanto ao _**tipo de segurança**_, podemos melhorar a segurança da nossa VM de duas formas: [Máquina virtual de inicialização confiável](http://go.microsoft.com/fwlink/?LinkId=2153371) e [Máquina virtual confidencial](https://aka.ms/ConfidentialVM). Para mais detalhes, é só clicar no link de cada tipo de segurança que você será redirecionado para a página oficial da microsoft.
- Em seguida, _**escolhemos a imagem do aplicativo ou sistema operacional**_ base da VM. O Azure oferece também a opção de escolher a arquitetura base para rodar seus aplicativos. As VMs baseadas em x64 fornecem a maior compatibilidade de software, enquanto as VMs baseadas em Arm64 oferecem até 50% melhor preço-desempenho do que as VMs x64 comparáveis.
- Por fim, escolhemos _**o tamanho da VM**_. Para maiores detalhes, clique no link: [Tamanhos de máquinas virtuais no Azure](https://learn.microsoft.com/pt-br/azure/virtual-machines/sizes/overview?tabs=breakdownseries%2Cgeneralsizelist%2Ccomputesizelist%2Cmemorysizelist%2Cstoragesizelist%2Cgpusizelist%2Cfpgasizelist%2Chpcsizelist).
## Conta de administrador
