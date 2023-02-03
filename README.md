# copier-protos-buf-connect

A copier template for starting with a [Buf Connect](https://connect.build/) enabled repo with optional Github Actions for publishing

# prerequisites

You will need an automation user of some kind with a token for Buf.build and NPM as well as an Github PAT if you want to use the Github Actions as they are.

Secret variables will need to be named (or adjusted by you after generation):

- AUTOMATON_PAT
- BUF_USER
- BUF_TOKEN
- NPM_TOKEN

# local generation?

If you want to try generating stuff locally (unsupported by catalystsquad), you'll need to do some go installs:

```
go install github.com/bufbuild/buf/cmd/buf@latest
go install github.com/fullstorydev/grpcurl/cmd/grpcurl@latest
go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
go install github.com/bufbuild/connect-go/cmd/protoc-gen-connect-go@latest
```
