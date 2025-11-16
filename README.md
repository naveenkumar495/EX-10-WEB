# Project Responsive Web Design using Bootstrap
## Date:16-11-2025

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.


## PROGRAM :

```
<!doctype html>
<html lang="en">

<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Scribble</title>

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>

<body class="bg-light">


    <nav class="navbar navbar-expand-lg bg-white border-bottom sticky-top">
        <div class="container">
            <a class="navbar-brand fw-bold" href="#">Scribb<span class="text-danger">le</span></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navMenu"
                aria-controls="navMenu" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navMenu">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item"><a class="nav-link" href="#">Explore</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Shots</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Designers</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Hire</a></li>
                </ul>
                <form class="d-flex me-2" role="search">
                    <input class="form-control" type="search" placeholder="Search" aria-label="Search">
                </form>
                <a href="#" class="btn btn-outline-secondary me-2">Sign in</a>
                <a href="#" class="btn btn-dark">Sign up</a>
            </div>
        </div>
    </nav>


    <header class="py-5 bg-white border-bottom">
        <div class="container">
            <div class="row align-items-center gy-4">
                <div class="col-lg-7">
                    <h1 class="display-5 fw-bold">Discover the world’s top designers & creatives</h1>
                    <p class="lead text-secondary">The leading community for showcasing and discovering design work.</p>


                    <form class="mt-3" role="search">
                        <div class="input-group input-group-lg">
                            <span class="input-group-text" id="search-addon">🔍</span>
                            <input type="text" class="form-control" placeholder="Search shots, designers, tags…"
                                aria-label="Search shots" aria-describedby="search-addon">
                            <button class="btn btn-dark" type="submit">Search</button>
                        </div>
                    </form>

                    <div class="mt-3">
                        <span class="me-2 text-secondary">Trending:</span>
                        <a href="#" class="badge text-bg-light rounded-pill me-2">UI</a>
                        <a href="#" class="badge text-bg-light rounded-pill me-2">Mobile</a>
                        <a href="#" class="badge text-bg-light rounded-pill me-2">Illustration</a>
                        <a href="#" class="badge text-bg-light rounded-pill me-2">Branding</a>
                        <a href="#" class="badge text-bg-light rounded-pill me-2">3D</a>
                    </div>
                </div>
                <div class="col-lg-5">

                    <img src="https://picsum.photos/800/500?random=1" alt="Featured design"
                        class="img-fluid rounded-4 shadow-sm">
                </div>
            </div>
        </div>
    </header>

    <section class="bg-white">
        <div class="container">
            <div class="d-flex flex-wrap align-items-center gap-2 py-3">
                <div class="dropdown">
                    <button class="btn btn-outline-secondary dropdown-toggle" data-bs-toggle="dropdown">Popular</button>
                    <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="#">Popular</a></li>
                        <li><a class="dropdown-item" href="#">New & Noteworthy</a></li>
                        <li><a class="dropdown-item" href="#">Most Discussed</a></li>
                    </ul>
                </div>
                <div class="dropdown">
                    <button class="btn btn-outline-secondary dropdown-toggle" data-bs-toggle="dropdown">All
                        time</button>
                    <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="#">Past day</a></li>
                        <li><a class="dropdown-item" href="#">Past week</a></li>
                        <li><a class="dropdown-item" href="#">Past month</a></li>
                        <li><a class="dropdown-item" href="#">All time</a></li>
                    </ul>
                </div>
                <div class="ms-auto">
                    <a class="btn btn-dark" href="#">Upload a shot</a>
                </div>
            </div>
        </div>
    </section>

    <main class="py-5">
        <div class="container">
            <div class="row g-4">

                <div class="col-12 col-sm-6 col-lg-4 col-xl-3">
                    <div class="card h-100 border-0 shadow-sm">
                        <img src="https://picsum.photos/600/400?random=2" class="card-img-top" alt="Shot 1">
                        <div class="card-body">
                            <h6 class="card-title mb-1">Fintech Dashboard</h6>
                            <p class="card-text small text-secondary mb-3">UI • Web</p>
                            <div class="d-flex align-items-center justify-content-between">
                                <div class="d-flex align-items-center gap-2">
                                    <img src="https://picsum.photos/40?random=21" class="rounded-circle" alt="Author"
                                        width="28" height="28">
                                    <span class="small">Alexis</span>
                                </div>
                                <div class="small text-secondary">❤ 1.2k</div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Card 2 -->
                <div class="col-12 col-sm-6 col-lg-4 col-xl-3">
                    <div class="card h-100 border-0 shadow-sm">
                        <img src="https://picsum.photos/600/400?random=3" class="card-img-top" alt="Shot 2">
                        <div class="card-body">
                            <h6 class="card-title mb-1">Travel App Concept</h6>
                            <p class="card-text small text-secondary mb-3">Mobile • Product</p>
                            <div class="d-flex align-items-center justify-content-between">
                                <div class="d-flex align-items-center gap-2">
                                    <img src="https://picsum.photos/40?random=22" class="rounded-circle" alt="Author"
                                        width="28" height="28">
                                    <span class="small">Priya</span>
                                </div>
                                <div class="small text-secondary">❤ 982</div>
                            </div>
                        </div>
                    </div>
                </div>


                <div class="col-12 col-sm-6 col-lg-4 col-xl-3">
                    <div class="card h-100 border-0 shadow-sm">
                        <img src="https://picsum.photos/600/400?random=4" class="card-img-top" alt="Shot 3">
                        <div class="card-body">
                            <h6 class="card-title mb-1">Mascot Illustration</h6>
                            <p class="card-text small text-secondary mb-3">Illustration</p>
                            <div class="d-flex align-items-center justify-content-between">
                                <div class="d-flex align-items-center gap-2">
                                    <img src="https://picsum.photos/40?random=23" class="rounded-circle" alt="Author"
                                        width="28" height="28">
                                    <span class="small">Diego</span>
                                </div>
                                <div class="small text-secondary">❤ 745</div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="col-12 col-sm-6 col-lg-4 col-xl-3">
                    <div class="card h-100 border-0 shadow-sm">
                        <img src="https://picsum.photos/600/400?random=5" class="card-img-top" alt="Shot 4">
                        <div class="card-body">
                            <h6 class="card-title mb-1">E-commerce Branding</h6>
                            <p class="card-text small text-secondary mb-3">Branding</p>
                            <div class="d-flex align-items-center justify-content-between">
                                <div class="d-flex align-items-center gap-2">
                                    <img src="https://picsum.photos/40?random=24" class="rounded-circle" alt="Author"
                                        width="28" height="28">
                                    <span class="small">Mina</span>
                                </div>
                                <div class="small text-secondary">❤ 1.1k</div>
                            </div>
                        </div>
                    </div>
                </div>


                <div class="col-12 col-sm-6 col-lg-4 col-xl-3">
                    <div class="card h-100 border-0 shadow-sm">
                        <img src="https://picsum.photos/600/400?random=6" class="card-img-top" alt="Shot 5">
                        <div class="card-body">
                            <h6 class="card-title mb-1">Crypto Wallet</h6>
                            <p class="card-text small text-secondary mb-3">UI • Fintech</p>
                            <div class="d-flex align-items-center justify-content-between">
                                <div class="d-flex align-items-center gap-2">
                                    <img src="https://picsum.photos/40?random=25" class="rounded-circle" alt="Author"
                                        width="28" height="28">
                                    <span class="small">Sara</span>
                                </div>
                                <div class="small text-secondary">❤ 869</div>
                            </div>
                        </div>
                    </div>
                </div>


                <div class="col-12 col-sm-6 col-lg-4 col-xl-3">
                    <div class="card h-100 border-0 shadow-sm">
                        <img src="https://picsum.photos/600/400?random=7" class="card-img-top" alt="Shot 6">
                        <div class="card-body">
                            <h6 class="card-title mb-1">SaaS Landing</h6>
                            <p class="card-text small text-secondary mb-3">Web • Marketing</p>
                            <div class="d-flex align-items-center justify-content-between">
                                <div class="d-flex align-items-center gap-2">
                                    <img src="https://picsum.photos/40?random=26" class="rounded-circle" alt="Author"
                                        width="28" height="28">
                                    <span class="small">Ken</span>
                                </div>
                                <div class="small text-secondary">❤ 503</div>
                            </div>
                        </div>
                    </div>
                </div>


                <div class="col-12 col-sm-6 col-lg-4 col-xl-3">
                    <div class="card h-100 border-0 shadow-sm">
                        <img src="https://picsum.photos/600/400?random=8" class="card-img-top" alt="Shot 7">
                        <div class="card-body">
                            <h6 class="card-title mb-1">Health App</h6>
                            <p class="card-text small text-secondary mb-3">Mobile</p>
                            <div class="d-flex align-items-center justify-content-between">
                                <div class="d-flex align-items-center gap-2">
                                    <img src="https://picsum.photos/40?random=27" class="rounded-circle" alt="Author"
                                        width="28" height="28">
                                    <span class="small">Ling</span>
                                </div>
                                <div class="small text-secondary">❤ 614</div>
                            </div>
                        </div>
                    </div>
                </div>


                <div class="col-12 col-sm-6 col-lg-4 col-xl-3">
                    <div class="card h-100 border-0 shadow-sm">
                        <img src="https://picsum.photos/600/400?random=9" class="card-img-top" alt="Shot 8">
                        <div class="card-body">
                            <h6 class="card-title mb-1">3D Icon Set</h6>
                            <p class="card-text small text-secondary mb-3">3D • Icons</p>
                            <div class="d-flex align-items-center justify-content-between">
                                <div class="d-flex align-items-center gap-2">
                                    <img src="https://picsum.photos/40?random=28" class="rounded-circle" alt="Author"
                                        width="28" height="28">
                                    <span class="small">Noah</span>
                                </div>
                                <div class="small text-secondary">❤ 458</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>


            <nav class="mt-4" aria-label="Shots pagination">
                <ul class="pagination justify-content-center">
                    <li class="page-item disabled"><span class="page-link">Previous</span></li>
                    <li class="page-item active" aria-current="page"><span class="page-link">1</span></li>
                    <li class="page-item"><a class="page-link" href="#">2</a></li>
                    <li class="page-item"><a class="page-link" href="#">3</a></li>
                    <li class="page-item"><a class="page-link" href="#">Next</a></li>
                </ul>
            </nav>
        </div>
    </main>


    <section class="py-5 bg-white border-top">
        <div class="container">
            <div class="row align-items-center gy-3">
                <div class="col-lg-8">
                    <h2 class="h3 fw-bold mb-1">Show your work to millions</h2>
                    <p class="mb-0 text-secondary">Join and upload your first shot today.</p>
                </div>
                <div class="col-lg-4 text-lg-end">
                    <a href="#" class="btn btn-dark btn-lg">Get started</a>
                </div>
            </div>
        </div>
    </section>

    <footer class="bg-white border-top">
        <div class="container py-4">
            <div class="d-flex flex-column flex-lg-row align-items-center justify-content-between gap-2">
                <div class="d-flex align-items-center gap-2">
                    <span class="fw-bold">Scribb<span class="text-danger">le</span></span>
                    <span class="text-secondary">© 2025</span>
                </div>
                <ul class="nav">
                    <li class="nav-item"><a class="nav-link px-2 text-secondary" href="#">About</a></li>
                    <li class="nav-item"><a class="nav-link px-2 text-secondary" href="#">Jobs</a></li>
                    <li class="nav-item"><a class="nav-link px-2 text-secondary" href="#">Support</a></li>
                    <li class="nav-item"><a class="nav-link px-2 text-secondary" href="#">Privacy</a></li>
                </ul>
                <div class="text-secondary small">
                    Built with Bootstrap • <span class="fw-semibold">AHAMADH SULAIMAN M</span>
                </div>
            </div>
        </div>
    </footer>


    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>

</html>

```



## OUTPUT:
<img width="1260" height="787" alt="image" src="https://github.com/user-attachments/assets/c160be3c-0034-4128-9944-b8d206bd6d00" />
<img width="1240" height="498" alt="image" src="https://github.com/user-attachments/assets/6ee5f101-70f9-46c1-b76c-14107a79543f" />


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
