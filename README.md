bitsurance
==========

Blockchain insurance protocol

Overview
--------

bitsurance is an experimental insurance protocol that enables
the instant purchase of insurance contracts covering some pre-specified
event. For illustrative purposes, we will assume the insurance being
purchased is for protection against earthquakes, but the protocol should
be generalizable to other forms of insurance.

Contracts are issued in the form of generic EarthquakeCoins, each of which
is redeemable for some agreed upon value in the event of an earthquake in
a pre-specified location. In order to validate a claim, redeemers
must provide proof of claim via a [ZipCodeCoin/ZipCodeAddress/some
other mechanism]. This decouples the value of an EarthquakeCoin from the
identity of its owner, making EarthquakeCoins generic, fungible units
and promoting a liquid secondary market while preventing bad actors from
fraudulently claiming loss from multiple locations. To that end, each
EarthquakeCoin may only be associated with one location to prevent
anyone from inflating the value of their coins by associating them with
payouts from multiple locations (for instance, by purchasing multiple
ZipCodeCoins).

The fee schedule will provide purchaser's with an estimate of the amount
of EarthquakeCoins they should purchase in order to make themselves whole.
This will vary with their location and subsequent risk exposure (since the
risk of loss from earthquakes is higher in Los Angeles than Nebraska, an
individual in Los Angeles would likely purchase more EarthquakeCoins than
her counterpart in  Nebraska). Payouts will be triggered when some condition
is met as determined by a trusted, 3rd party feed.

Premiums are used to purchase [GoldCoins or some basket of stable, inflation
resistant assets] which back the EarthquakeCoins and which are used to
finance any claims. The insurer's fee is [calculated as a percentage of
premiums/charged upon issuance of an EarthquakeCoin/determined via an
inflationary follow-on issuance of EarthquakeCoins].

EarthquakeCoins [expire/do not expire]. Coverage may be purchased on a
[monthly/biannual/annual] basis.
