FROM public.ecr.aws/lambda/python:latest

COPY app.py requirements.txt ${LAMBDA_TASK_ROOT}/

RUN python -m pip install -r requirements.txt -t .

# Command can be overwritten by providing a different command in the template directly.
CMD ["app.lambda_handler"]
