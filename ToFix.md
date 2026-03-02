1. more greenhand-friendly, save for lots of terms
2. 
```mermaid
graph TD
    A[用户输入命令] --> B[1. 词法分析/解析]
    B --> C[2. 别名展开 Alias Expansion]
    C --> D[3. 各种扩展 Expansion]
    D --> E[4. 重定向处理 Redirection]
    E --> F[5. 命令查找 Command Lookup]
    F --> G{找到命令了吗?}
    G -- 是 --> H[6. 执行 Execution]
    G -- 否 --> I[报错: Command not found]
    H --> J[7. 返回结果并显示到终端]
```

3. shells comparison, terminal bash os relations

4. CLI moved forward
bash syntax and tools

5. bindkey
alias(optional)

6. redirect pipeline illustrations

7. bash is an interpretive language whose interpreter is bash.
shebang
source script file vs execute script file

8. zsh, fish(optional)
