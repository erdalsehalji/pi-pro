<style>
  #log {
    background-color: lightslategray;
    padding-bottom: 10 px;
    text-align: center;
  }

  #reg {
    background-color: rgb(19, 227, 36);
    text-align: center;
  }

  #dob {}
</style>

<template>

  <div>

    <nav class="navbar navbar-expand-lg navbar navbar-dark bg-primary">
      <a class="navbar-brand" href="#">Navbar</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav"
        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item active">
            <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Features</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Pricing</a>
          </li>
          <li class="nav-item">
            <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
          </li>
        </ul>
      </div>
    </nav>

    <br>



    <div class="container">
      <div class="row">

        <div id="raz" class="col-1">

        </div>

        <div id="log" class="col-3">
          <form>
            <div class="form-group">
              <label for="exampleInputEmail1">Email address</label>
              <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp"
                placeholder="email">
              <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
            </div>
            <div class="form-group">
              <label for="exampleInputPassword1">Password</label>
              <input type="password" class="form-control" id="exampleInputPassword1" placeholder="password">
            </div>
            <button type="submit" class="btn btn-primary">Submit</button>
          </form>
        </div>

        <div id="raz" class="col-1">

        </div>

        <div id="reg" class="col-6">

          <div class="form-row">

            <div class="form-group col-md-6">
              <label for="inputEmail4">Ime</label>
              <input type="email" class="form-control" id="inputEmail4" placeholder="ime">
            </div>

            <div class="form-group col-md-6">
              <label for="inputEmail4">Prezime</label>
              <input type="email" class="form-control" id="inputEmail4" placeholder="prezime">
            </div>

            <div class="form-group col-md-6">
              <label for="inputEmail4">Email</label>
              <input type="email" class="form-control" id="inputEmail4" placeholder="email">
            </div>

            <div class="form-group col-md-6">
              <label for="inputPassword4">Password</label>
              <input type="Password" id="inputpassword" placeholder="Password" class="form-control">
            </div>


            <div id="dob" class="form-group col-md-6">
              <label for="inputState">Spol</label>
              <select id="inputState" class="form-control">
                <option selected>Odaberi...</option>
                <option>M</option>
                <option>Ž</option>
              </select>
            </div>

            <div id="dob" class="form-group col-md-6">
              <label for="inputState">Dob</label>
              <select id="inputState" class="form-control">
                <option selected>Odaberi...</option>
                <option>1</option>
                <option>...</option>
              </select>
            </div>

          </div>
          <button type="submit" class="btn btn-primary">Registracija</button>
          <br>
        </div>

        </form>
      </div>



    </div>

    <div id="raz" class="col-1">

    </div>





  </div>
  </div>
</template>