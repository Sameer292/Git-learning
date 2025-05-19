# Writing better commits with conventional commits

`<type>[optional scope]:<description>`

`[optional body]`

`[optional footer(s)]`


### Type:
1. fix - use for bug fixes
2. feat - use for code features
3. build
4. chore
5. ci
6. docs
7. style
8. refactor
9. test 

### Optional scope
> It is to provide additional information. It should be a noun and inside a parentheses

> eg: fix(parser): , feat(api):

#### ! to draw attention to breaking changes

> eg: feat!: , feat(api)!:

### description
> This is a short message about the commit

> This should be writte in imperative. eg: ~~adds feature~~ || ~~added feature~~ 
✅ **add** feature ✅


### Optional body
> Explain the changes

> Not all commits are complex enough that they need a body


### Footer
> It follows the body with one blank line and must use a word token followed by a colon(:) or a hashtag(#)
 
> Can be used for other metadata options

> Also optional 



### To create changelog from this

> npm install -D standard-version

> add "release":"standard-version" in package.json scripts

> Run npm run release