<section>
<div class="card">
    <div class="card-body">
      <h5 class="card-title"><slot name="title"></slot></h5>
      <h6 class="card-subtitle mb-2 text-muted"><slot name="subtitle"></slot></h6>
      <p class="card-text"><slot name="text"></slot></p>
    </div>
  </div>
</section>

<style>
    .card {
        display: block;
        margin-left: auto !important;
        margin-right: auto !important;
        width: 65%;
        margin: 0;
        margin-bottom: 20px;
        margin-top: 20px;
        border-radius: 20px;
        background: rgba(0, 0, 0, 0.6);
        border: none;
        color: white !important;
    }

    h6 {
      color: lightblue !important;
    }

</style>