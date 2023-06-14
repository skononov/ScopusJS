# ScopusJS.html
Browser app on JavaScript for searching scientific publications via free Scopus Search API. 
Download _ScopusJS.html_ on your PC and open in any modern web browser. No special permissions are needed. To use it one has to obtain an Elsevier's development API key on https://dev.elsevier.com/ (free registration) and enter it in the form. For frequent use one may include an API key in the code as a value of the input#apikey element.

# ScopusPureJS.html
Scopus and Pure clients combined. Check a Pure CRIS for publications found in Scopus and show Pure ID along with document IDs from Scopus.
Download _ScopusPureJS.html_ on your PC and open in any modern web browser. To use it one has to obtain an Elsevier's development API key on https://dev.elsevier.com/ (free registration) and enter it in the form. For frequent use one may include an API key in the code as a value of the input#apikey element. 
One also needs to indicate also three consts in the JS code:

    //==================== Pure client code ====================
    const pureEndpoint = 'https://<Pure-API-URL>/research-outputs'; // указать адрес сервиса Pure WS вместо <Pure-API-URL>
    const pureApiKey = '<Valid API key>'; // указать API-ключ для доступа к Pure WS без авторизации вместо <Valid API key>
    const pureUrlTemplate = 'https://<Pure-URL>/admin/editor/dk/atira/pure/api/shared/model/researchoutput/editor/{pureType}editor.xhtml?scheme=&type=&id={pureId}'; // указать адрес бэкенда Pure вместо <Pure-URL>
