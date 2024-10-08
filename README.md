# Let's Play with Go Language

As usual, let's go to <https://killercoda.com/playgrounds/scenario/ubuntu> to get an Ubuntu machine (for 60 minutes).

## Install Go

Reference(s): <https://go.dev/doc/install>

Check what is the latest version of Go at <https://go.dev/dl>, which is Go 1.23.0 at the time of writing.

Check if any previous version of Go is installed trying the `go` command:

```text
go version
```

or by looking at the `VERSION` file whithin the `/usr/local/go` folder (if it exists):

```text
more /usr/local/go/VERSION
```

Then, if needed, download the latest version of Go from <https://go.dev/dl>. At the time of writing it is `1.23.0`:

```text
wget https://go.dev/dl/go1.23.0.linux-amd64.tar.gz
```

remove the previous version of Go

```text
rm -rf /usr/local/go
```

and extract the archive you just downloaded into `/usr/local`, creating a fresh Go tree in `/usr/local/go`:

```text
tar -C /usr/local -xzf go1.23.0.linux-amd64.tar.gz
```

Add the `/usr/local/go/bin` folder to the PATH environment variable by adding the following line:

```text
export PATH=$PATH:/usr/local/go/bin
```

into your `$HOME/.profile` file

```text
vi $HOME/.profile
```

and apply the change

```text
source $HOME/.profile
```

Verify that you've installed the latest version of Go:

```text
go version
```

Now you can write your first "Hello, World!" Go program following <https://go.dev/doc/tutorial/getting-started>.
