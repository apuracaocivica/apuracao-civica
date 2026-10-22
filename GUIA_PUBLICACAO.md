# Publicação — Apuração Cívica

## 0. Registrar o domínio

A confirmação de que `apuracaocivica.com.br` está disponível **não significa que já seja seu**. Registre e pague o domínio em https://registro.br/ antes de configurar DNS.

## 1. Criar repositório

No https://github.com/new crie repositório público `apuracao-civica` (sem espaços/acentos). Envie **os arquivos na raiz**: `index.html`, `CNAME`, `.nojekyll` e opcionalmente os MDs. O arquivo `index.html` não deve ficar dentro de uma pasta.

## 2. Ativar GitHub Pages

Abra seu repositório > Settings > Pages > Build and deployment > Source: Deploy from a branch > Branch: main > / (root) > Save. Confira o endereço temporário https://SEU_USUARIO.github.io/apuracao-civica/ .

## 3. Vincular domínio próprio no GitHub primeiro

Ainda em Settings > Pages > Custom domain, defina `apuracaocivica.com.br` e Save (mesmo que o arquivo CNAME já exista). O GitHub recomenda verificar a propriedade do domínio nas configurações da conta, quando possível.

## 4. Configurar DNS no provedor que administra sua zona

Se estiver usando DNS do Registro.br, abra o domínio no painel e a edição de zona DNS. Para o domínio raiz `@`, adicione quatro registros **A** distintos:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

Opcionalmente configure `www` como `CNAME` apontando para `SEU_USUARIO.github.io` (troque pelo usuário real). Caso já existam registros conflitantes, revise antes de alterar. Se o DNS estiver hospedado em outro serviço, faça os ajustes lá, não necessariamente no Registro.br.

## 5. HTTPS e conferência

Depois de os registros DNS propagarem, vá a GitHub > Settings > Pages e habilite **Enforce HTTPS** quando disponível. Abra https://apuracaocivica.com.br/ e teste também no celular. DNS pode levar até 24 horas. Se a página não funcionar, confira Actions/Pages, raiz do repositório e registros DNS.

## 6. Lembretes

- Este HTML não atualiza automaticamente, não possui banco e representa uma amostra de outubro/2026.
- Enquanto o protótipo não estiver plenamente auditado, manter a identificação de laboratório e não indexação pelos buscadores.
- O registro do domínio e a marca no INPI são processos separados.

Fontes: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site e https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
