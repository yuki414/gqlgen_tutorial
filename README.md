# gqlgen_tutorial

## Command

When changing a file, you can generate by this command.
```
go run github.com/99designs/gqlgen generate
```

Note: at first, the below command is needed to use.
```
go run github.com/99designs/gqlgen init
```


## About files

#### Automatically generated
- `graph/generated.go`
- `graph/model/model_gen.go`
  - Type and input is defined here.
- `graph/schema.resolver.go`
  - It's a resolver file based on the request.

These three files are generated by gen command after changing schema file.

#### Manually created
- `graph/resolver.go`
- `graph/schema.graphqls`
  - This is a main file. Based on this, other files is generated.
- `graph/gqlgen.yml`
  - It's config file of gqlgen itself.
