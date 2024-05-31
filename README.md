```markdown
## Bem-vindo(a) ao perfil do Felipe 😁
* 👨‍💻 C# Backend developer 
* 📚💻Sou um desenvolvedor com experiência em Flutter, Getx, Dart, C#, SQL Server, Bootstrap, JavaScript, ASP.NET Framework MVC e jQuery. Sou apaixonado por tecnologia e sempre busco aprender mais sobre as últimas tendências e ferramentas.
* https://felipealvesnn.github.io/Portf-lio/
  
<div>
  <a href="https://github.com/Felipealvesnn">
    <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Felipealvesnn&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true"/>
    <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Felipealvesnn&hide=scss,less&layout=compact&langs_count=6&theme=tokyonight"/>
  </a>
</div>
  
<div style="display: inline_block"><br>
  <img align="center" alt="Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  <img align="center" alt="HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
  <img align="center" alt="C#" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg">
  <img align="center" alt="Flutter" height="30" width="40" src="https://www.vectorlogo.zone/logos/flutterio/flutterio-icon.svg">
  <img align="center" alt="Dart" height="30" width="40" src="https://www.vectorlogo.zone/logos/dartlang/dartlang-icon.svg">
</div>

<br>
 
### Me siga nas redes abaixo!
 
<div> 
  <a href="mailto:felipe.alvesnn@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
  <a href="https://www.linkedin.com/in/felipealvesnn/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
</div>

![Snake animation](https://github.com/Felipealvesnn/Felipealvesnn/blob/output/github-contribution-grid-snake.svg)
```

Verifique se a URL da imagem da cobra (`https://github.com/Felipealvesnn/Felipealvesnn/blob/output/github-contribution-grid-snake.svg`) está correta. Caso contrário, você pode precisar regenerar a animação ou verificar o script de geração da cobra para garantir que ele esteja funcionando corretamente.

Para regenerar a animação, você pode usar um script GitHub Actions. Aqui está um exemplo de como você pode configurar isso no seu repositório:

1. Crie um arquivo `.github/workflows/snake.yml` no seu repositório com o seguinte conteúdo:

```yaml
name: Generate Snake Animation

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout Repository
        uses: actions/checkout@v2
      - name: Generate Snake Animation
        uses: Platane/snk@v2.0.1
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          output: dist/github-contribution-grid-snake.svg
      - name: Commit and Push Changes
        run: |
          git config --global user.name 'github-actions[bot]'
          git config --global user.email '41898282+github-actions[bot]@users.noreply.github.com'
          git add -A
          git commit -m 'Generate snake animation'
          git push
```
