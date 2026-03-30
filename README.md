# Meu Projeto CI
## Validação Parte 3 (DAG)

Stage  Job ID             Job name           Workflow name       Workflow file              Events                
0      setup-e-lint       setup-e-lint       Pipeline Principal  02-pipeline-principal.yml  push                  
1      scan-de-seguranca  scan-de-seguranca  Pipeline Principal  02-pipeline-principal.yml  push                  
1      testes-unitarios   testes-unitarios   Pipeline Principal  02-pipeline-principal.yml  push                  
2      build-e-deploy     build-e-deploy     Pipeline Principal  02-pipeline-principal.yml  push  

## Validação Parte 4 (Paralelismo)

É possível comprovar que os jobs testes-unitarios e scan-de-seguranca rodaram em paralelo observando que ambos iniciam ao mesmo tempo no terminal e seus logs aparecem intercalados durante a execução, indicando execução simultânea em contêineres separados.
