Por que a Secret aparece no log como ** e a variável aparece
normalmente?
Os variavis não são cinsiderados sensivis mas os secret são.

O Job deploy_app consegue ler a variável BUILD_VERSION criada no Job
build_app? Por quê?
Não
Cada job no GitHub Actions roda em um ambiente isolado, uma máquina separada.
As variáveis criadas com $GITHUB_ENV só existem dentro do mesmo job.
