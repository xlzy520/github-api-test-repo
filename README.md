# github-api-test-repo
用于测试GitHub Rest API的项目


### 创建一个新分支
`https://api.github.com/repos/xlzy520/github-api-test-repo/git/refs` `POST` 
参数
```js
{
    "owner": "xlzy520",
    "repo": "github-api-test-repo",
    "ref": "refs/heads/main1",
    "sha": "7ec56d693f0c17d5501154d45569c64ee857ae96" // from的分支的最新的一个commit的hash值
}
```
