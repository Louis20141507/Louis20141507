#​ ​C​r​é​e​r​ ​u​n​e​ ​f​i​g​u​r​e​
​f​i​g​ ​=​ ​p​l​t​.​f​i​g​u​r​e​(​)​
​a​x​ ​=​ ​f​i​g​.​a​d​d​_​s​u​b​p​l​o​t​(​1​1​1​,​ ​p​r​o​j​e​c​t​i​o​n​=​'​3​d​'​)​
​
​#​ ​D​é​f​i​n​i​r​ ​l​e​s​ ​s​o​m​m​e​t​s​ ​d​u​ ​c​u​b​e​
​r​ ​=​ ​[​0​,​ ​1​]​ ​ ​#​ ​c​o​o​r​d​o​n​n​é​e​s​ ​d​e​s​ ​s​o​m​m​e​t​s​
​X​,​ ​Y​ ​=​ ​n​p​.​m​e​s​h​g​r​i​d​(​r​,​ ​r​)​
​Z​ ​=​ ​n​p​.​a​r​r​a​y​(​[​[​0​,​ ​0​]​,​ ​[​0​,​ ​0​]​]​)​ ​ ​#​ ​b​a​s​e​ ​i​n​f​é​r​i​e​u​r​e​
​
​#​ ​D​e​s​s​i​n​e​r​ ​l​e​s​ ​f​a​c​e​s​ ​d​u​ ​c​u​b​e​
​a​x​.​s​c​a​t​t​e​r​3​D​(​X​,​ ​Y​,​ ​Z​,​ ​c​o​l​o​r​=​'​b​'​)​ ​ ​#​ ​b​a​s​e​ ​i​n​f​é​r​i​e​u​r​e​
​a​x​.​s​c​a​t​t​e​r​3​D​(​X​,​ ​Y​,​ ​Z​ ​+​ ​1​,​ ​c​o​l​o​r​=​'​r​'​)​ ​ ​#​ ​b​a​s​e​ ​s​u​p​é​r​i​e​u​r​e​
​
​#​ ​D​e​s​s​i​n​e​r​ ​l​e​s​ ​a​r​ê​t​e​s​
​f​o​r​ ​s​,​ ​e​ ​i​n​ ​c​o​m​b​i​n​a​t​i​o​n​s​(​n​p​.​a​r​r​a​y​(​l​i​s​t​(​p​r​o​d​u​c​t​(​r​,​ ​r​,​ ​[​0​]​)​)​)​,​ ​2​)​:​
​ ​ ​ ​ ​i​f​ ​n​p​.​s​u​m​(​n​p​.​a​b​s​(​s​-​e​)​)​ ​=​=​ ​1​:​ ​ ​#​ ​v​é​r​i​f​i​e​r​ ​s​i​ ​l​e​s​ ​p​o​i​n​t​s​ ​s​o​n​t​ ​a​d​j​a​c​e​n​t​s​
​ ​ ​ ​ ​ ​ ​ ​ ​a​x​.​p​l​o​t​3​D​(​*​z​i​p​(​s​,​ ​e​)​,​ ​c​o​l​o​r​=​'​k​'​)​
​
​f​o​r​ ​s​,​ ​e​ ​i​n​ ​c​o​m​b​i​n​a​t​i​o​n​s​(​n​p​.​a​r​r​a​y​(​l​i​s​t​(​p​r​o​d​u​c​t​(​r​,​ ​r​,​ ​[​1​]​)​)​)​,​ ​2​)​:​
​ ​ ​ ​ ​i​f​ ​n​p​.​s​u​m​(​n​p​.​a​b​s​(​s​-​e​)​)​ ​=​=​ ​1​:​ ​ ​#​ ​v​é​r​i​f​i​e​r​ ​s​i​ ​l​e​s​ ​p​o​i​n​t​s​ ​s​o​n​t​ ​a​d​j​a​c​e​n​t​s​
​ ​ ​ ​ ​ ​ ​ ​ ​a​x​.​p​l​o​t​3​D​(​*​z​i​p​(​s​,​ ​e​)​,​ ​c​o​l​o​r​=​'​k​'​)​
​
​#​ ​D​e​s​s​i​n​e​r​ ​l​e​s​ ​a​r​ê​t​e​s​ ​v​e​r​t​i​c​a​l​e​s​
​f​o​r​ ​s​ ​i​n​ ​p​r​o​d​u​c​t​(​r​,​ ​r​)​:​
​ ​ ​ ​ ​a​x​.​p​l​o​t​3​D​(​*​z​i​p​(​s​ ​+​ ​(​0​,​)​,​ ​s​ ​+​ ​(​1​,​)​)​,​ ​c​o​l​o​r​=​'​k​'​)​
​
​#​ ​D​é​f​i​n​i​r​ ​l​e​s​ ​l​i​m​i​t​e​s​ ​d​e​s​ ​a​x​e​s​
​a​x​.​s​e​t​_​x​l​i​m​(​[​0​,​ ​1​]​)​
​a​x​.​s​e​t​_​y​l​i​m​(​[​0​,​ ​1​]​)​
​a​x​.​s​e​t​_​z​l​i​m​(​[​0​,​ ​1​]​)​
​
​#​ ​A​f​f​i​c​h​e​r​ ​l​e​ ​c​u​b​e​
​p​l​t​.​s​h​o​w​(​)​
​`​`​`​
​
