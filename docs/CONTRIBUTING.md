# Guia de Contribuição

Obrigado pelo interesse em contribuir com este projeto! 🎉

## Fluxo de trabalho

1. Faça um fork do repositório
2. Crie uma branch a partir de `main`:
   ```bash
   git checkout -b feature/minha-feature
   ```
3. Faça suas alterações e commits seguindo as convenções abaixo
4. Push para o seu fork
5. Abra um Pull Request seguindo o template

## Convenções de commit

Use [Conventional Commits](https://www.conventionalcommits.org/):

- `feat:` nova funcionalidade
- `fix:` correção de bug
- `docs:` mudanças na documentação
- `style:` formatação (sem mudança de lógica)
- `refactor:` refatoração de código
- `test:` adição ou correção de testes
- `chore:` tarefas de manutenção
- `data:` mudanças nos dados ou pipelines de dados

Exemplo: `feat: adiciona pipeline de limpeza de dados de vendas`

## Padrões de código

- Siga o estilo [PEP 8](https://peps.python.org/pep-0008/)
- Use `black` para formatação automática
- Use `isort` para organizar imports
- Use `flake8` para linting
- Escreva docstrings para funções e classes
- Adicione type hints quando possível

```bash
# Antes de fazer commit
black src/ tests/
isort src/ tests/
flake8 src/ tests/
pytest tests/
```

## Notebooks

- Limpe os outputs antes de fazer commit (`Restart Kernel and Clear All Outputs`)
- Use nomes descritivos com prefixo numérico: `01-exploracao-inicial.ipynb`
- Mova código reutilizável dos notebooks para módulos em `src/`

## Dados

- **Nunca** faça commit de dados sensíveis ou pessoais
- Documente a origem e o processamento dos dados

## Dúvidas?

Abra uma issue com a tag `question` ou entre em contato com os mantenedores.
