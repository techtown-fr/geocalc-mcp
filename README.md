# geocalc-mcp

Serveur MCP GéoCalc prêt à l'emploi pour la formation TechTown « Coder avec l'IA et Claude Code » (TP 8).
Transport STDIO, trois outils : `list_shapes`, `get_formula`, `validate_calculation`.

## Prérequis

JDK 21 ou plus récent (`java -version`). Ni Maven ni compilation nécessaires.

## Utilisation

1. Téléchargez `geocalc-mcp-server.jar` depuis la [dernière release](https://github.com/techtown-fr/geocalc-mcp/releases/latest).
2. À la racine du projet Angular GéoCalc :

```bash
claude mcp add --scope project --transport stdio geocalc \
  -- java -jar /chemin/absolu/vers/geocalc-mcp-server.jar
```

3. Dans Claude Code, lancez `/mcp` et vérifiez que `geocalc` expose les trois outils.

Empreinte SHA-256 publiée avec chaque release (`shasum -a 256 geocalc-mcp-server.jar`).
