# Vpython_Solar_System_Model

# Solar-System-Model-in-Vpython-glowscript-

The creation of the code behind the
solar system animation 2.0 stems from the
3D animation of vpython. Each planetary
object is initially defined as a sphere and
given intrinsic properties that define how it
looks and how it operates. The sphere
function inside vpython allows for the
customization of each object the user wishes
to implement into their animation.
The program initially starts off with
basic variables that are defined as the radius
and orbital radius of each planet. These
values define each planet are taken from the
NASA planet fact website to ensure accurate
cosmological values. These variables that
define each sphere are then placed inside of
the sphere function along with their
appropriate name.
The vpython sphere function allows
for additional customization such as its
position vector, radius, color, texture, make
trail, and make trail colors. The texture
feature of the sphere function requires the
coder to either choose from a very limited
pre-implemented texture option that is
already inside of the vpython module, or to
set the texture variable equal to a url of the
text image packet. For example, the Earth
texture is already inside of vpython and can
be called using texture = textures.earth
(which is the only planet texture), but for the
Sun’s texture it must be defined as a specific
url such as texture =
"https://i.imgur.com/XdRTvzj.jpg".
The initial variable for the planet's
orbital radius is the average distance from
the planet to the Sun and is technically only
one dimensional. In order to incorporate the
radius distance into the 3D vector array, and
allow it to rotate around the Sun, the
position vector must be placed in the x and z
axis due to the 3D sphere rotating around a
2D orbital plane. To ensure that the planet
does not simply move in a straight line like a
box, but rather an orbital circle, some
trigonometric functions must be used and
implemented in a loop in order to
continuously change its position radially
around the center of the solar system which
is defined as the vector (0,0,0).
Before creating the loop that makes
the animation of the planets going around
the Sun, each planet’s sphere must have an
initial angle value of 0 that will continuously
be added in the loop within each planet’s
respective position vector. When inside of
the loop function, the planet’s x and z vector
plane will continuously loop through the
angle value. For the x vector plane it will be
the planet’s radius multiplied by the cosine
of the angle and for the z vector plane will
be the planet’s radius multiplied by the sine
of the angle. This function inside of an
infinite loop will cause each of the spheres
to continuously rotate around the Sun at a
rate defined by the user.
Planets however do not just rotate
around the Sun, but also around their own
axis (except for Mercury). When defining
the rotational function of each planet’s
sphere, vpython has a built-in rotation
function that will cause an object to rotate
about its axis. The rotation function of each
sphere requires an angle and an axial vector.
Each planet has a defined epsilon value that
is based on the ecliptic coordinates for their
axial tilt rotation. In vpython the degree
values that are taken from the NASA
website must be converted into radians and
vectorized in order to communicate with the
vpython module. Each planet’s coordinates
correlate to their given rotational tilt values
with respect to the 2D orbital plane that
revolves around the Sun.
The animation system that vpython
is built off of is entirely vectorized and thus
the function for rotating each planet must
take into account the x, y, and z coordinates
in a 3D plane. In order to tilt each planet
based on their given axial tilts, the ecliptic
coordinates must be placed in the x and y
plane. Likewise in order to rate the entire
sphere around the center of the system, their
orbital coordinates must correlate to the x
and z plane.
The last component to accurately
scale the solar system is to ensure that each
planet rotates around the Sun at their
respective rate. Each planet’s orbital rate is
based on how many Earth days it takes to
orbit the Sun. These values are then inverted
and continuously subtracted from time 0 in
the loop function to simulate their respective
orbital periods.
The last method that was used in the
project is the vpython graphing function.
This feature was added to the animation in
order to give specific value for the position
of each planet in real time. This simple
function has powerful uses due to the fact
that one can compare the distances from one
planet to another based on their current
position around the Sun. This idea (but more
advanced) is what NASA uses in order to
determine when the most optimal time is to
launch satellites to other worlds in order to
conserve time and resources. The user
should note however that in order to see the
full orbit of Pluto for example, the rate of
the loop must be increased dramatically in
order to see it in a reasonable time frame, or
one would have to wait for the actual time it
takes for Pluto to orbit the Earth which is
approximately 250 years!

The purpose of the project was to
construct a real scaled simulation of the
planets orbiting the Sun. The base code in
this program proved to do just that, and
although this simulation does not include
every possible factor that goes into making
the planets orbit the Sun, it does give the
user an overall perspective of the scale of
our solar system. The vast rates and
distances that separate each planet from one
another cannot be visualized without a direct
animation to show the ratios of one planet's
distance versus another.
The vpython module has many
powerful capabilities that allow users to
customize the aesthetics and behavior of a
given set of objects. Even though this
module allows for some basic movement
animations of 3D objects, it is primitive
compared to other modernized graphic
programs that are designed to to handle
large amounts of data flow to create
complex and continuously evolving
animations with arduous equations running
in the background.
The solar system animation
portrayed for this project only touches the
surface for what computer programs can
achieve when attempting to model the
universe around us. This animation depicts
only 9 spheres moving in a circle around a
10th sphere and yet the code behind it is
very complex compared to what is being
seen. One can now only imagine the code
and calculations that go into creating a real
life scale of the Milky Way with over 200
billion stars or an animation of the entire
universe that consists of over 2 trillion
galaxies and distances that the human mind
cannot even comprehend.
This is where having a
supercomputer powered by an artificial
intelligence calculating trillions of equations
over multiple years is required to obtain a
remotely accurate depiction of the universe
as a whole. The relatively small scale of the
solar system is enough to where the vpython
program begins to hit its upper limits on
what it can achieve but with enough time
and creativity, an accurate and relatively
pleasing looking animation can be attained.
The program constructed in this
project attempts to exploit as much of
vpython’s capabilities as possible without
crashing the system. Further progression and
alternate simulations can still be achieved in
the vpython environment, all that is needed
is further creativity to create increasingly
dynamic and complex celestial animation
