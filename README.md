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

### 获取分支列表详情
```https://api.github.com/repos/xlzy520/github-api-test-repo/git/refs/heads``` `GET`
#### 响应
```js
[
    {
        "ref": "refs/heads/main",
        "node_id": "REF_kwDOGlcLja9yZWZzL2hlYWRzL21haW4",
        "url": "https://api.github.com/repos/xlzy520/github-api-test-repo/git/refs/heads/main",
        "object": {
            "sha": "331540a9a2661993e58b4361929246edefcfbbb4",
            "type": "commit",
            "url": "https://api.github.com/repos/xlzy520/github-api-test-repo/git/commits/331540a9a2661993e58b4361929246edefcfbbb4"
        }
    },
    {
        "ref": "refs/heads/main1",
        "node_id": "REF_kwDOGlcLjbByZWZzL2hlYWRzL21haW4x",
        "url": "https://api.github.com/repos/xlzy520/github-api-test-repo/git/refs/heads/main1",
        "object": {
            "sha": "6f28e66927be1b91ec391a466953d91f18e98838",
            "type": "commit",
            "url": "https://api.github.com/repos/xlzy520/github-api-test-repo/git/commits/6f28e66927be1b91ec391a466953d91f18e98838"
        }
    }
]
```
