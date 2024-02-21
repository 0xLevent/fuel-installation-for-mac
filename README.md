# fuel-mac-kurulumu

## Adım 1: Terminali Açma


## Adım 2: Homebrew Kurulumu
Aşağıdaki kodu terminale yapıştırarak Homebrew kurulumunu gerçekleştirin.

``
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
``
## Adım 3: curl Kurulumu
``
brew install curl
``

##Adım 4: Git Kurulumu

`brew install git`

##Adim 5: Rust Kurulumu 
kodu yapistirdiktan sonra gelen ekranda y yazip entera basmaniz gerekiyor

`curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`

## Adim 6: rust versiyon kontrol edelim

`rustup --version`



##Adim 7: Fuel Araç Seti Kurulumu
Fuel araç setini kurmak için fuelup-init betiğini yüklemeniz gerekmektedir. Eğer komut sizden yolu değiştirmenizi isterse, y ve "Enter" tuşlarına basarak yolu değiştirin.
`curl --proto '=https' --tlsv1.2 -sSf https://install.fuel.network/fuelup-init.sh | sh`

Kurulum işleminin başarılı olup olmadığını kontrol etmek için aşağıdaki komutu çalıştırın.
`fuelup --version`


Araç setinizin güncel olduğundan emin olun.
`fuelup self update`

Beta-4 araç setini kurmak için aşağıdaki komutu çalıştırın.

`fuelup toolchain install beta-4`

Beta-4'ü varsayılan araç seti olarak ayarlamak için aşağıdaki komutu çalıştırın.
`fuelup default beta-4`

Kullandığınız araçların ve sürümlerinin listesini görmek için aşağıdaki komutu çalıştırın.

`fuelup show`




## İlk Sway Projemizi Oluşturalım

Yeni bir klasör oluşturmak için aşağıdaki komutları sırayla yapıştırın:

`mkdir petition-app`

`cd petition-app`

`forc new petition-contract`


## Bu komutların ardından terminalinizde aşağıdaki gibi bir çıktı görmelisiniz:

To compile, use `forc build`, and to run tests use `forc test`

----

Read the Docs:
- Sway Book: https://docs.fuel.network/docs/sway
- Forc Book: https://docs.fuel.network/docs/forc
- Rust SDK Book: https://docs.fuel.network/docs/fuels-rs
- TypeScript SDK: https://docs.fuel.network/docs/fuels-ts

Join the Community:
- Follow us @SwayLang: https://twitter.com/SwayLang
- Ask questions on Discourse: https://forum.fuel.network/

Report Bugs:
- Sway Issues: https://github.com/FuelLabs/sway/issues/new

Şimdi petition-app adlı dosyanızı VS Code ile açarak Fuel'de geliştirme yapabilirsiniz!






