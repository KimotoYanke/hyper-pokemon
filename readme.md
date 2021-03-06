<h1 align="center">
  <img src="https://cdn.rawgit.com/klauscfhq/hyper-pokemon/221ba5d5/media/logo.png" width="30%"><br/>Hyper Pokemon
</h1>

<h4 align="center">
  🌈 Tailor-made Pokémon themes for your Hyper terminal
</h4>

<div align="center">
      <a href="https://github.com/klauscfhq/hyper-pokemon">
        <img src="https://cdn.rawgit.com/champloohq/hyper-pokemon/36074d40/media/screen.png" alt="Hyper Pokemon" width="95%">
      </a>
</div>

[![Build Status](https://travis-ci.org/klauscfhq/hyper-pokemon.svg?branch=master)](https://travis-ci.org/klauscfhq/hyper-pokemon) [![Dependency Status](https://dependencyci.com/github/klauscfhq/hyper-pokemon/badge)](https://dependencyci.com/github/klauscfhq/hyper-pokemon) [![Gitter](https://img.shields.io/gitter/room/nwjs/nw.js.svg)](https://gitter.im/klauscfhq/hyper-pokemon) [![XO code style](https://img.shields.io/badge/code_style-XO-5ed9c7.svg)](https://github.com/klauscfhq/hyper-pokemon) [![Latest version](https://badge.fury.io/gh/klauscfhq%2Fhyper-pokemon.svg)](https://github.com/klauscfhq/hyper-pokemon/releases) [![npm](https://img.shields.io/npm/dt/hyper-pokemon.svg)](https://github.com/klauscfhq/hyper-pokemon) [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/bnb/awesome-hyper)

## Contents

- [Description](#description)
- [Install](#install)
- [Usage](#usage)
- [Options](#options)
- [Available Themes](#available-themes)
- [Related](#related)
- [Team](#team)
- [License](#license)

## Description

Made for Pokémon enthusiasts by Pokémon enthusiasts ❤

All of the wonderful Pokémon backgrounds were created by the amazing [Teej/TopHat](https://pldh.net/gallery/the493) & [MapleRose](https://twitter.com/PokeWalls).

Do you enjoy this project? Maybe you love **Star Wars**, **Yoda** or **Darth Vader**?<br/>Then, you will also love our [Hyper Star Wars](https://github.com/klauscfhq/hyper-star-wars) theme project. Go have a peek.

Come over to our [Gitter](https://gitter.im/klauscfhq/hyper-pokemon) channel to share your thoughts on the project or to just say hi.

## Vote the next Region

Vote for the Pokémon Region you want to see themes from next.<br/>
In essence, this poll will determine the creation order of all Pokémon Regions.<br/>
The poll will be kept alive until the project's completion, when all **600+** themes will be available.

[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BMH8W2ETBFXQ9H6PSS0X9VZ8/Johto)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BMH8W2ETBFXQ9H6PSS0X9VZ8/Johto/vote)
[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BMH8W2ETBFXQ9H6PSS0X9VZ8/Hoenn)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BMH8W2ETBFXQ9H6PSS0X9VZ8/Hoenn/vote)
[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BMH8W2ETBFXQ9H6PSS0X9VZ8/Sinnoh)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BMH8W2ETBFXQ9H6PSS0X9VZ8/Sinnoh/vote)
[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BMH8W2ETBFXQ9H6PSS0X9VZ8/Unova)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BMH8W2ETBFXQ9H6PSS0X9VZ8/Unova/vote)
[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BMH8W2ETBFXQ9H6PSS0X9VZ8/Kalos)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BMH8W2ETBFXQ9H6PSS0X9VZ8/Kalos/vote)

<sub>Poll powered by [tj/gh-polls](https://github.com/tj/gh-polls)</sub>

## Install

### Using the plugin manager - `hpm-cli`

Firstly, ensure you have [Hyper](https://github.com/zeit/hyper/releases) and [Node.js](https://nodejs.org) installed in your system.<br/>
Then simply do the `npm` dance to get `hpm-cli`

```bash
# fire up a terminal and type
$ npm install -g hpm-cli
```

Once done with that, it's time to install the `hyper-pokemon` theme.

```bash
# run the hyper plugin manager
$ hpm install hyper-pokemon
```

### Manually through `.hyper.js`

Add `hyper-pokemon` to the plugins list in your `~/.hyper.js` config file and restart Hyper.

```js
plugins: ['hyper-pokemon']
```

## Usage

Once you have installed `hyper-pokemon`, it's time to set your favorite theme.

Go to your `~/.hyper.js` and add the `pokemon` and `pokemonSyntax` options below the `colors` object, and define your theme of choice.

Here is a quick example, where we choose the `gengar` ![](pokecursors/gengar.gif) theme, with a `unibody` color for the window header & dark terminal tabs.

```js
config: {
    //...
    colors: {
    //...
    },
    pokemon: 'gengar', // Define your favorite pokemon theme
    pokecursor: 'true', // Activate your theme's pokecursor
    pokemonSyntax: 'dark', // Define the color of the terminal tabs
    unibody: 'true', // Define the color of the Hyper window header
    poketab: 'false', // Deactivate your theme's poketab
    //...
}
```

![Gengar Example](media/example.png)

To get the exact same look, install Google's [`Roboto Mono`](https://fonts.google.com/specimen/Roboto+Mono) font as well as [`oh-my-zsh`](http://ohmyz.sh/) and choose [`pure`](https://github.com/sindresorhus/pure) as your zsh prompt.

## Options

### `pokemon`

Using this option you can choose your pokémon background along with it's tailor-made syntax color.

The assignable values are:

- `pokemon name` - choose any of the [available Pokémon themes](#available-themes) by defining the Pokémon name.<br/><br/>**i.e.** `pokemon: 'charizard'`, `pokemon: 'pikachu'`, `pokemon: 'blastoise'` **etc**<br/><br/>

- `random` - randomly selects a Pokémon theme from the **whole list** of available Pokémons, each time you fire up a new Hyper terminal session.<br/><br/>
**i.e.** `pokemon: 'random'`<br/><br/>

- `pokemon type` - randomly selects a Pokémon theme from only a **specific Pokémon type**, each time you fire up a new Hyper terminal session. You can view all available Pokémon types [here](#available-themes).<br/><br/>
**i.e.** `pokemon: 'fire'`, `pokemon: 'water'`, `pokemon: 'grass'` **etc**<br/><br/>

- `pokemon trainer` - randomly selects a Pokémon theme from only a **specific Pokémon Trainer's party**, each time you fire up a new Hyper terminal session. You can view all available Pokémon Trainer [here](#available-themes).<br/><br/>
**i.e.** `pokemon: 'ash'`, `pokemon: 'jessie'`, `pokemon: 'gary'`, `pokemon: 'erika'` **etc**<br/><br/>

- `pokemon party` - randomly selects a Pokémon theme/theme option from a **defined array** holding **custom multiple themes/theme options**, each time you fire up a new Hyper terminal session. Any from the available Pokémon **themes**, **types** & **trainers** can be chosen.<br/><br/>
**i.e.**
	- `pokemon: ['articuno', 'zapdos', 'moltres', 'mewtwo', 'mew']`
	- `pokemon: ['random', 'fire', 'water', 'grass', 'ash', 'pikachu']`
	- `pokemon: ['lance', 'brock', 'bruno', 'gary', 'legendary', 'dragonite']` **etc**<br/><br/>

### `pokecursor`

Replace the regular terminal cursor with an animated `.gif` that matches the current pokemon theme.

The assignable values are:

- `pokecursor: 'true'` - enable your theme's pokecursor
- `pokecursor: 'false'` - revert to the cursor's original appearance

Also, completely omitting the `pokecursor` option from your `.hyper.js` will have the same effect as defining it and setting it to `false`. (**default state**)

<div align="center">
		<br/>
			<a href="">
				<img src="https://github.com/champloohq/hyper-pokemon/blob/master/media/pokecursor.gif" alt="Hyper Pokemon - Pokecursor" width="80%">
			</a>
		<br/>
		<br/>
</div>

### `pokemonSyntax`

Here you can define the color of the terminal tabs.

The assignable values are:

- `pokemonSyntax: 'light'` - choose it if your pokémon theme is of a more light color
- `pokemonSyntax: 'dark'` - go for it if you are using a darker pokémon theme

![Pokemon Syntax](media/pokemon-syntax.png)

### `unibody`

Choose whether or not you want the Hyper windows header color to be the same as the background pokémon theme.

The assignable values are:

- `unibody: 'true'` - choose it for a unibody color theme
- `unibody: 'false'` - go for it if you like your terminal more colorful

In addition, completely omitting the `unibody` option from your `.hyper.js` will have the same effect as defining it and setting it to `true`. (**default state**)

![Unibody](media/unibody.png)

### `poketab`

Choose whether or not you want an animated `.gif` that matches your current pokemon theme, to accompany your active Hyper terminal tab.

The assignable values are:

- `poketab: 'true'` - enable your theme's poketab
- `poketab: 'false'` - disable your theme's poketab

Also, completely omitting the `poketab` option from your `.hyper.js` will have the same effect as defining it and setting it to `false`. (**default state**)

<div align="center">
		<br/>
			<a href="">
				<img src="https://github.com/champloohq/hyper-pokemon/blob/master/media/poketab.gif" alt="Hyper Pokemon - Poketab" width="80%">
			</a>
		<br/>
		<br/>
</div>

## Available Themes

You can view all the available themes [here](https://klauscfhq.github.io/hyper-pokemon).

#### Pokémon Types

> List of all available Pokémon types

<details>
<summary>Pokémon Types</summary>

<br/>

* `Legendary`
* `Starter`
* `Fire`
* `Water`
* `Grass`
* `Poison`
* `Flying`
* `Bug`
* `Electric`
* `Ground`
* `Fairy`
* `Normal`
* `Psychic`
* `Ghost`
* `Rock`
* `Ice`
* `Dragon`
* `Fighting`
* `Steel`

<br/>

</details><br/>

#### Pokémon Trainers

> List of all available Pokémon trainers

<details>
<summary>Pokémon Trainers</summary>

<br/>

* `Ash`
* `Agatha`
* `Blaine`
* `Brock`
* `Bruno`
* `Erika`
* `Gary`
* `Giovanni`
* `James`
* `Jessie`
* `Koga`
* `Lance`
* `Lorelei`
* `Surge`
* `Misty`
* `Sabrina`

<br/>

</details><br/>

## Related

More awesome Hyper plugins.

- [Hyper Star Wars](https://github.com/klauscfhq/hyper-star-wars) - 🚀 Super awesome, your Hyper terminal shall look.

## Team

Meet the team and all the [contributors](https://github.com/klauscfhq/hyper-pokemon/blob/master/authors.md).<br/>

[![Klaus Sinani](https://avatars.githubusercontent.com/u/12670537?s=130)](https://github.com/klauscfhq) | [![Mario Sinani](https://avatars.githubusercontent.com/u/29512262?s=130)](https://github.com/mariocfhq) | [![George Baxopoulos](https://avatars.githubusercontent.com/u/19195396?s=130)](https://github.com/georgebax) | [![Thanasis Gkanos](https://avatars.githubusercontent.com/u/18072542?s=130)](https://github.com/ThanasisGkanos) | [![Konstantinos Mitropoulos](https://avatars.githubusercontent.com/u/24499401?s=130)](https://github.com/tsikos7) | [![Gabriel Tibúrcio](https://avatars.githubusercontent.com/u/5959178?s=130)](https://github.com/tibuurcio)
--- | --- | --- | --- | --- | ---
[Klaus Sinani](https://github.com/klauscfhq) | [Mario Sinani](https://github.com/mariocfhq) | [George Baxopoulos](https://github.com/georgebax) | [Thanasis Gkanos](https://github.com/ThanasisGkanos) | [Konstantinos Mitropoulos](https://github.com/tsikos7) | [Gabriel Tibúrcio](https://github.com/tibuurcio)

## License

[MIT](https://github.com/klauscfhq/hyper-pokemon/blob/master/license.md)
