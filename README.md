# Stuba Cancellation Fees

## Case #1

We receive two dates with the same price

```xml

<Result id="752296769-0">
    <Room>
        <RoomType code="85063005" text="Standard Plus Room"/>
        <MealType code="1000041" text="Room only"/>
        <Price amt="165.36"/>
        <Guests>
            <Adult id="-2" first="" last="">
                <Price amt="165.36"/>
            </Adult>
        </Guests>
        <CanxFees>
            <Fee from="2023-08-14T07:50:15.7206933+01:00">
                <Amount amt="165.36000000000000000000000000"/>
            </Fee>
            <Fee from="2023-08-15T00:00:00">
                <Amount amt="165.36000000000000000000000000"/>
            </Fee>
        </CanxFees>
        <Messages/>
        <CancellationPolicyStatus>Refundable</CancellationPolicyStatus>
    </Room>
</Result>
```

## Case #2

We receive a single price without any dates

```xml

<Result id="752295588-8">
    <Room>
        <RoomType code="9112249" text="Deluxe room + Free Wifi"/>
        <MealType code="1000041" text="Room only"/>
        <Price amt="95.72"/>
        <Guests>
            <Adult id="-536870921" first="" last="">
                <Price amt="95.72"/>
            </Adult>
        </Guests>
        <CanxFees>
            <Fee>
                <Amount amt="95.72000000000000000000000000"/>
            </Fee>
        </CanxFees>
        <Messages/>
        <CancellationPolicyStatus>Refundable</CancellationPolicyStatus>
    </Room>
</Result>
```

## Case #3

We receive two different prices with two different dates

```xml

<Result id="752295326-8">
    <Room>
        <RoomType code="9112246" text="Superior room + Free Wifi"/>
        <MealType code="1000041" text="Room only"/>
        <Price amt="83.04"/>
        <Guests>
            <Adult id="-536870920" first="" last="">
                <Price amt="83.04"/>
            </Adult>
        </Guests>
        <CanxFees>
            <Fee from="2023-08-30T00:00:00+01:00">
                <Amount amt="83.04000000000000000000000000"/>
            </Fee>
            <Fee from="2023-08-30T00:00:00">
                <Amount amt="41.520000000000000000000000000"/>
            </Fee>
        </CanxFees>
        <Messages/>
        <CancellationPolicyStatus>Refundable</CancellationPolicyStatus>
    </Room>
</Result>
```

## Case #4

We receive two prices one with a date and one without a date

```xml

<Result id="752294257-4">
    <Room>
        <RoomType code="9112249" text="Deluxe room + Free Wifi"/>
        <MealType code="1000041" text="Room only"/>
        <Price amt="48.10"/>
        <Guests>
            <Adult id="-536870920" first="" last="">
                <Price amt="48.10"/>
            </Adult>
        </Guests>
        <CanxFees>
            <Fee>
                <Amount amt="48.099999999999999999999999999"/>
            </Fee>
            <Fee from="2023-08-14T07:39:37.4646759+01:00">
                <Amount amt="48.099999999999999999999999999"/>
            </Fee>
        </CanxFees>
        <Messages/>
        <CancellationPolicyStatus>Refundable</CancellationPolicyStatus>
    </Room>
</Result>
```