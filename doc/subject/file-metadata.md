文件元数据
--------

edp允许我们在文件中声明`文件元数据`。

`文件元数据`为用户声明文件的相关信息，edp的各种模块在处理文件（如loader配置自动同步）时，可以读取`文件元数据`信息，并根据信息执行不同的处理策略。

`文件元数据`一般声明在文件注释内部，从而避免对文件产生影响。edp支持以`JSON`形式的`文件元数据`，并允许以下4种注释声明方式：

    <!-- edp: 
    {
        webpath: "/path"
    }
    -->

    /* edp: 
     * {
     *     webpath: "/path"
     * }
     */

    // edp: 
    // {
    //     webpath: "/path"
    // }

    # edp: 
    # {
    #     webpath: "/path"
    # }
