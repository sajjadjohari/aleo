# aleo
aleo is best network in defi and deploy smart contract

Hello guys

aleo smart contract
open putty and open codes below:
Install prerequisites
------------------------------------------------------------------
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

source $HOME/.cargo/env

rustup install stable

rustup update stable

rustup default stable

git clone https://github.com/AleoHQ/leo
cd leo

apt install clang gcc libssl-dev pkg-config

cargo install --path .

git clone https://github.com/AleoHQ/snarkOS.git --depth 1
cd snarkOS

./build_ubuntu.sh

cargo install --path .

------------------------------------------------------------------
To get fast, you must send the following message format to the following number:

number: +18678885688
massage: send 50 credits to aleo1fl2kum48tz2sssx2x5t779ydhsrt45xnn65kvxll3qzh8mheru9q3va4q6

------------------------------------------------------------------

cd $HOME

mkdir demo_deploy_Leo_app && cd demo_deploy_Leo_app

(Put your wallet address between two marks " )
WALLETADDRESS=""

APPNAME=helloworld_"${WALLETADDRESS:4:6}"

leo new "${APPNAME}"

PATHTOAPP=$(realpath -q $APPNAME)

cd $PATHTOAPP && cd ..

(Put your wallet PRIVATEKEY between two marks " )
PRIVATEKEY=""

(To get record, you must go to the message you received through the number and copy the record part in the output section and go to site aleo.tools and send record and view key and COPY code from site and put it between two marks  " .)
RECORD=""

snarkos developer deploy "${APPNAME}.aleo" --private-key "${PRIVATEKEY}" --query "https://vm.aleo.org/api" --path "./${APPNAME}/build/" --broadcast "https://vm.aleo.org/api/testnet3/transaction/broadcast" --fee 600000 --record "${RECORD}"
------------------------------------------------------------------
good luck my friends
