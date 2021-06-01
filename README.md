# sops-sample

## Usage

```sh
$ git config diff.sopsdiffer.textconv "sops -d"

sops -p BCE6E1D2A509156191BA016FDF0B5C535207EF1E secretdir/secretfile
sops updatekeys secretdir/secretfile


sops --rotate --in-place --add-pgp <PGP> --encrypt secret.yaml --verbose

sops --output secret.enc.yaml --encrypt secret.yaml
sops --output secret.yaml --decrypt secret.enc.yaml

sops --output-type binary --output secretdir/secretfile.enc.bin --input-type binary --encrypt secretdir/secretfile --verbose
```

> [mozilla/sops #727 gpg.mozilla.org is broken (probably for good) #727](https://github.com/mozilla/sops/issues/727)  
> [mozilla/sops #613 Is there a way to integrate with Visual Studio Code? #613](https://github.com/mozilla/sops/issues/613)  
> [mozilla/sops #598 Argument order for --extract #598](https://github.com/mozilla/sops/issues/598)  
> [mozilla/sops #716 sops -e data --output data.enc doesn't output to ./data.enc as expected #716](https://github.com/mozilla/sops/issues/716)  
> [mozilla/sops #782 --output <value> does not have any effect #782](https://github.com/mozilla/sops/issues/782)  
