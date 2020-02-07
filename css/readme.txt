I denna mapp placeras css-dokument.

async function getPerson() {
    let respose = await fetch('js/data.json');
    let data = await response.json();
    return data;
}

getPerson().then(dat => {
    console.log(`Hej jag heter ${dat.person1.name} $
    {dat.person1.lastName} och jag är en agent = $
    {dat.person1.agent}`);

    console.log(`Hej ${dat.person2.name}${dat.person2.ond}`);
}); 