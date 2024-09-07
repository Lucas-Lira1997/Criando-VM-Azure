# **Criando-VM-Azure**
Guia para criação de máquina virtual (VM) utilizando o Microsoft Azure

## **Sumário**
1. **Primeiros passos**
2. **Detalhes do projeto**
3. **Detalhes da instância**
4. **Conta de administrador**
5. **Regras de portas de entrada**
6. **Marcas**
7. **Revisar + Criar**

## 1. **Primeiros passos**
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
## 4. **Conta de administrador**
- No _**tipo de autenticação**_, podemos optar pela conectividade através de par de chaves SSH ou por senha. Nesta etapa, optei por usar o par de chaves SSH no formato Ed25519 para autenticação do usuário.
- Logo abaixo, podemos definir nosso _**nome de usuário**_, ou seja, o administrador da VM.
- Por último, podemos escolher o _**nome do par de chaves**_ ou deixarmos como já vem pré-definido, _**nome da máquina_key**_.
## 5. **Regras de portas de entrada**
Nesta etapa, iremos selecionar quais portas de rede da máquina virtual podem ser acessadas via internet pública.
- Na opção de portas de entrada pública, irei selecionar SSH (22). Você poderá alterar as regras de porta de entrada na VM > Página de rede.
- Por fim, iremos clicar em _**avançar: Marcas >**_ no canto inferior esquerdo.
## 6. **Marcas**
Marcas são elementos de metadados que você aplica aos recursos do Azure. Elas são pares chave-valor que ajudam você a identificar recursos com base em configurações relevantes para sua organização. Para saber mais sobre, clique aqui [Marcas](https://learn.microsoft.com/pt-br/azure/azure-resource-manager/management/tag-resources?wt.mc_id=azuremachinelearning_inproduct_portal_utilities-tags-tab)!
No momento, irei deixar em branco esse campo.
## 7. **Revisar + Criar**
Essa é a última etapa de criação da VM, onde é fornecido uma estimativa do custo da sua VM. Entretanto, recomendo que consulte a calculadora de preços do Azure para uma estimativa mais precisa de acordo com suas necessidades nos serviços oferecidos -> [Calculadora de preços](http://go.microsoft.com/fwlink/?LinkId=2189385)!
No meu caso, a estimativa de custo foi de 0.0151 U$D/hora.
Recomendo também, a leitura para obter mais detalhes dos termos legais e as políticas de privacidade associadas à ofertas do Marktplace da Microsoft. [Termos do Azure Marktplace](https://azure.microsoft.com/support/legal/marketplace-terms/)!
- Após a revisão dos dados da VM e a leitura dos termos legais, é só clicarmos em _**Criar**_ no canto inferior esquerdo. Pronto, agora sua máquina virtual será criada e você poderá utilizar os serviços oferecidos pela Microsoft Azure!
