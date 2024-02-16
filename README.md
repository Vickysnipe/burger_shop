### How to run the project
======================
SETTING UP
To run contracts, instantiate contracts and more, we need to download the Ink! CLI. Open your terminal and run rustup component add rust-src.
After the process finishes, run cargo install --force --locked cargo-contract.
To verify the package is installed in your pc, run cargo contract -V or cargo contract --version. You also run cargo contract --help to see other available commands.

Next, we install substrate-contracts-node. This is a simple substrate blockchain configured for smart contract functionality using contracts-pallets. You can use this instead of a Testnet.

You could also install it using cargo instead, by running cargo install contracts-node --git https://github.com/paritytech/substrate-contracts-node.git --tag v0.23.0 --force --locked.
To verify that it is downloaded, run substrate-contracts-node -V also to check for other commands run substrate-contracts-node --help.

Let's create our project, we'll call it "burger_shop", in your project's directory, run cargo contract new burger_shop.
This should create a project and generate an ink! smart contract template.


 Run the project
`cargo run`
 Build the project
   `cargo contract build --release`
 Check for errors
   `cargo check`
