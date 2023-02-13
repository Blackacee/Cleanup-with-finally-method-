# Cleanup-with-finally-method-

var loadingData = true;
fetch('/data')
 .then(result => processData(result.data))
 .catch(error => console.error(error))
 .finally(() => {
 loadingData = false;
)};
