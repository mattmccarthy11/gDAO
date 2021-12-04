# gBTC variables & functions

address carbonOffset;

address assetToOffset;

uint RATIO;

Function checkOffsetRatio(uint numAssetToOffset, uint numCarbonOffset) --> bool

```
if( hasEnoughCarbonOffsets(uint numAssetToOffset, uint numCarbonOffset) && hasEnoughAssetToOffset(uint numAssetToOffset, uint numCarbonOffset)
```

Function hasEnoughCarbonOffsets(uint numAssetToOffset, uint numCarbonOffset) --> bool

```
if( carbonOffset / RATIO =! numAssetToOffset)
return false
```

Function hasEnoughAssetToOffset(uint numAssetToOffset, uint numCarbonOffset) --> bool

```
if( numAssetToOffset * RATIO =! carbonOffset)
return false
```



```
Contract
{
address carbonOffset;
address assetToOffset;
uint RATIO;
}

Constructor()
{
ratio = 191;
}

Function confirmAndDeposit
If( ratioAtoken(carbonOffset,assetToOffset) && ratioBtoken(amountA,assetToOffset) && isBothApproved  == true)
Return deposit(carbonOffset,assetToOffset)
 
Function checkRatioCarbonOffset
if RatioAtoken(carbonOffset,assetToOffset) == false 
return string 
{
Return ‘please deposit’ +carbonOffset/ ratio +’of’ +assetToOffset
}

Function RatioCarbonOffset(carbonOffset,assetToOffset)
Return bool 
{
If( carbonOffset / RATIO =! assetToOffset)
Return false
}

Function checkRatioAssetToOffset
if RatioBtoken(carbonOffset,assetToOffset) == false 
return string 
{
Return ‘please deposit’ +assetToOffset * ratio +’of’ +carbonOffset
}

Function checkRatioAssetToOffset(carbonOffset,assetToOffset)
Return bool
{
If( assetToOffset * ratio =! carbonOffset)

Return false
}

isBothApproved

Function approveSpendCarbonOffset
Return bool

Function approveSpendAssetToOffset
Return bool 

```
