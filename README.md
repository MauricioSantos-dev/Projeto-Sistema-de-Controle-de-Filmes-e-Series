<h1>Projeto: Gerenciador/Controle de filmes e séries</h1>
<br>
<h2>Objetivos do Projeto</h2>
<br>
•	Um sistema feito para gerenciar e controlar filmes e séries, categorizando a princípio como "vistos" e "não vistos", com intuito de ajudar o usuário a tanto manter suas experiências pessoais de assistir determinada mídia documentada de uma certa forma, quanto compartilhar dita experiência para outros usuários, descrevendo e recomendando, ou até mesmo criticando essa mídia. <br>
•	O objetivo principal é adicionar funcionalidades mais complexas de sites alternativos para ser uma opção objetivamente mais completa de catalogar e controlar filmes e séries vistos ou não vistos.<br><br>

Requisitos Funcionais 
<br>
🔹 Personalização avançada de perfil e privacidade
O sistema deverá permitir que os usuários personalizem seus perfis de forma mais detalhada, controlando tanto a aparência quanto as informações exibidas. Isso inclui a possibilidade de escolher quais dados serão públicos (como listas, avaliações, histórico de visualização) e quais permanecerão privados ou visíveis apenas para seguidores.
Além disso, o usuário poderá configurar preferências de privacidade, como:
•	Perfil público ou privado 
•	Exibição de atividades recentes no feed 
•	Controle sobre quem pode comentar ou interagir com seu conteúdo 
Essa funcionalidade busca oferecer maior controle ao usuário sobre sua identidade dentro da plataforma, tornando a experiência mais segura e personalizada.

🔹 Customização de capas de conteúdos (filmes/séries/listas)
<br>
O sistema deverá permitir que os usuários personalizem visualmente os conteúdos adicionados às suas listas, incluindo a possibilidade de alterar capas padrão por imagens próprias.
Essa funcionalidade poderá incluir:
•	Upload de imagens personalizadas para capas 
•	Escolha entre capas oficiais (via API) ou personalizadas 
•	Aplicação de capas em listas criadas pelo usuário 
O objetivo é proporcionar uma experiência mais visual e única, permitindo que cada usuário organize seu conteúdo de forma mais criativa e individualizada.

🔹 Acompanhamento detalhado de séries (checklist e progresso)
<br>
Para conteúdos do tipo série, o sistema deverá oferecer um controle mais granular do progresso do usuário, permitindo o acompanhamento por episódios e temporadas.
As funcionalidades incluem:
•	Marcação de episódios assistidos (checklist) 
•	Indicação automática do próximo episódio a assistir 
•	Cálculo de progresso total da série em porcentagem 
•	Visualização do progresso por temporada 
Esse recurso visa melhorar significativamente o controle de consumo de séries, tornando mais fácil acompanhar conteúdos longos e evitando que o usuário se perca no progresso.

🔹 Interação social entre usuários (comentários e avaliações)
<br>
A plataforma deverá permitir a interação entre usuários por meio de funcionalidades sociais, semelhantes às encontradas em aplicações já consolidadas.
Entre as interações disponíveis, destacam-se:
•	Publicação de avaliações (notas e reviews) em filmes e séries 
•	Sistema de comentários em conteúdos e avaliações 
•	Possibilidade de curtir ou reagir a avaliações de outros usuários 
•	Feed de atividades exibindo ações recentes (ex: assistiu, avaliou, comentou) 
Esse conjunto de funcionalidades tem como objetivo tornar a plataforma mais dinâmica e engajadora, incentivando a troca de opiniões e a construção de uma comunidade ativa em torno do consumo de mídia.
<br>
<br>
Requisitos Não Funcionais 
<br>
🔹 Desempenho
<br>
O sistema deve apresentar tempos de resposta rápidos, garantindo uma boa experiência ao usuário mesmo com grande volume de dados (como listas, avaliações e episódios).
•	O tempo de resposta das requisições principais (login, carregamento de perfil, listas e backlog) deve ser inferior a 2 segundos 
•	O carregamento de páginas com listas extensas (ex: backlog ou episódios de séries) deve ser otimizado com paginação ou carregamento sob demanda (lazy loading) 

🔹 Usabilidade
<br>
A interface deve ser intuitiva, responsiva e de fácil navegação, permitindo que usuários consigam utilizar as principais funcionalidades sem dificuldade.
•	O sistema deve ser responsivo, funcionando corretamente em dispositivos móveis, tablets e desktops 
•	As ações principais (adicionar ao backlog, marcar episódio, avaliar conteúdo) devem ser acessíveis em poucos cliques 
•	A navegação deve seguir padrões conhecidos de UI/UX 

🔹 Segurança
<br>
O sistema deve garantir a proteção dos dados dos usuários, especialmente considerando as configurações de privacidade dos perfis.
•	As senhas devem ser armazenadas de forma criptografada 
•	O sistema deve utilizar autenticação segura (ex: JWT) 
•	Os dados privados do usuário devem respeitar as configurações de visibilidade definidas no perfil 
•	Deve haver proteção contra acessos não autorizados 

🔹 Escalabilidade
<br>
O sistema deve ser capaz de suportar o aumento do número de usuários e dados sem perda significativa de desempenho.
•	A arquitetura deve permitir expansão futura (ex: mais usuários, mais interações) 
•	O sistema deve suportar crescimento no volume de avaliações, comentários e conteúdos 

🔹 Disponibilidade
<br>
O sistema deve estar disponível para acesso na maior parte do tempo, garantindo confiabilidade para os usuários.
•	O sistema deve ter disponibilidade mínima de 95% 
•	Deve haver tratamento de erros para evitar falhas críticas 

🔹 Manutenibilidade
<br>
O código deve ser organizado e estruturado de forma que facilite manutenção e evolução do sistema.
•	Utilização de arquitetura organizada (ex: MVC) 
•	Código modular e reutilizável 
•	Documentação básica das APIs e componentes 

🔹 Compatibilidade
<br>
O sistema deve funcionar corretamente nos principais navegadores modernos.
•	Compatível com Google Chrome, Firefox e Edge 
•	Deve seguir padrões web (HTML5, CSS3, ES6+) 

🔹 Confiabilidade
<br>
O sistema deve garantir consistência dos dados, especialmente no progresso de séries e listas.
•	O progresso de episódios não deve ser perdido após atualização 
•	As avaliações e listas devem ser salvas corretamente no banco de dados 
•	Deve haver validação de dados antes do armazenamento 

🔹 Armazenamento e mídia
<br>
Considerando que você quer upload de capas:
•	O sistema deve suportar upload de imagens com limite de tamanho (ex: até 5MB) 
•	As imagens devem ser armazenadas de forma otimizada 
•	Deve haver validação de formato (PNG, JPG) 

🔹 Privacidade 
<br>
•	O usuário deve poder controlar quem vê suas listas e atividades 
•	O sistema deve respeitar as configurações de perfil (público/privado) em todas as funcionalidades sociais

O que está incluso no protótipo:
- Roadmap / Power-up do Trello
- GitHub (Repositório e Pipelines)
- README.md / Documentação do projeto
