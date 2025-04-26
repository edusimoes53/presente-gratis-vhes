# App Free Gift Buy X Get Y para Shopify

Este app permite que lojistas Shopify configurem promoções do tipo "Compre X e Ganhe Y", onde ao adicionar determinados produtos ao carrinho em uma quantidade mínima, outros produtos são automaticamente adicionados como brinde.

## Funcionalidades

- Detecção automática de produtos específicos no carrinho
- Adição automática de produtos gratuitos como brinde
- Interface de administração para configurar regras personalizadas
- Opções para definir quantidade mínima de produtos
- Suporte para selecionar variantes específicas de produtos

## Instalação

Este repositório contém o código-fonte do app em formato ZIP. Para instalar:

1. Extraia o arquivo `shopify-free-gift-app.zip`
2. Configure as credenciais do Shopify:
   - Edite o arquivo `src/lib/cartIntegration.ts`
   - Substitua as variáveis de ambiente por seus valores reais:
     ```typescript
     const SHOPIFY_API_KEY = "seu_id_do_cliente";
     const SHOPIFY_API_SECRET = "sua_chave_secreta";
     const SHOPIFY_SHOP = "sua-loja.myshopify.com";
     ```
3. Hospede o app em um serviço como Netlify, Vercel ou similar
4. Configure as URLs no Shopify Partners:
   - URL do app: https://seu-app-hospedado.com
   - URL de redirecionamento: https://seu-app-hospedado.com/auth/callback

## Estrutura do Projeto

- `src/components/admin/`: Componentes da interface de administração
- `src/components/cart/`: Componentes de integração com o carrinho
- `src/lib/`: Bibliotecas e utilitários
- `src/pages/`: Páginas do Next.js
- `docs/`: Documentação completa

## Documentação

Para mais detalhes, consulte os arquivos na pasta `docs/`:
- `manual_usuario.md`: Instruções detalhadas de uso
- `guia_instalacao.md`: Guia passo a passo de instalação
- `guia_desenvolvedor.md`: Documentação técnica para desenvolvedores

## Suporte

Para suporte ou dúvidas, entre em contato com o desenvolvedor.
