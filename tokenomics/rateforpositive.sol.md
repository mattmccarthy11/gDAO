# rateForPositive.sol

this contract takes a positive asset and sets the amount of offsets it requires.

this is ownable by the dao offsetRate voting contract&#x20;



//the amount of offset to apply to a coal mined bitcoin

uint coalOffsetRate;

//the amount of offset to apply to a natural gas mined bitcoin

uint natGasOffsetRate;



// this function takes in an address with a carbon positive BTC NFT&#x20;

// it sets the offset amount dependent on the metadata{coal, natural gas}

functions calculateOffset

if NFT metadata == COAL

\--> return coalOffsetRate;

else&#x20;

\-->return natGasOffsetRate;



//getters&#x20;

function getCoalOffsetRate()

function getNatGasOffsetRate()



//setting the coalOffsetRate

function setCoalOffsetRate(newRate)

coalOffsetRate = newRate;

//setting the natGasOffsetRate

function setNatGasOffsetRate(newRate)

natGasOffsetRate = newRate;

