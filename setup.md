### Generate new Icons

1. Place the SVG files in the `[root]/svgs` directory. 
2. Rename the name to be PascalCase without numbers spaces or other special chracters. [a-zA-Z]. For a batch renaming use below commands:

```bash
for file in *; do mv $file ${file//OLD_VALUE/NEW_VALUE}; done
// verify the command initially 
for file in *; do echo mv $file ${file//OLD_VALUE/NEW_VALUE}; done
```

3. Execute `npm run build`
4. Update package version and publish with `npm run release`
