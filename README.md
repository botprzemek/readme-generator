# readme-generator
typescript project which generates svg with actual data

var svg = document.createElementNS("http://www.w3.org/2000/svg", "svg");
var path1 = document.createElementNS("http://www.w3.org/2000/svg", 'path');
var path2 = document.createElementNS("http://www.w3.org/2000/svg", 'path');

svg.setAttribute("aria-hidden","true");
svg.setAttribute('viewbox', '0 0 24 24');
svg.setAttribute('width', '24px');
svg.setAttribute('height', '24px');

path1.setAttribute('d', 'M0 0h24v24H0z');
path1.setAttribute('fill', 'none');

path2.setAttribute('d', 'M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 17.93c-3.95-.49-7-3.85-7-7.93 0-.62.08-1.21.21-1.79L9 15v1c0 1.1.9 2 2 2v1.93zm6.9-2.54c-.26-.81-1-1.39-1.9-1.39h-1v-3c0-.55-.45-1-1-1H8v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41c2.93 1.19 5 4.06 5 7.41 0 2.08-.8 3.97-2.1 5.39z');
path2.setAttribute('fill', '#2962ff');

svg.appendChild(path1);
svg.appendChild(path2);
document.body.appendChild(svg);
